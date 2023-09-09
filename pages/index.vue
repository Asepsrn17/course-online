<template>
  <div id="app">
    <TheHeader :searchQuery="searchQuery" @search="handleSearch" @update-search="updateSearch"
      @category="updateCategory" />
    <div class="container-card">
      <div class="container-card-body">
        <CardItem v-for="(course, index) in filteredCourses" :course="course" :key="index" />
        <h5 v-if="filteredCourses.length === 0">Kursus tidak ditemukan</h5>
      </div>
    </div>
    <TheFooter />
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue';
import TheFooter from '@/components/TheFooter.vue';
import CardItem from '@/components/Card/CardItem.vue';

export default {
  components: {
    TheHeader,
    TheFooter,
    CardItem,
  },
  data() {
    return {
      courses: [
        {
          title: 'Javascript Dasar',
          description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime mollitia,molestiae quas vel sint commodi repudiandae consequuntur voluptatum laborum numquam blanditiis harum quisquam eius sed odit fugiat iusto fuga praesentium optio, eaque rerum',
          image: require('@/assets/jsdasar.jpg'),
          price: 'free',
          jumlahPelajaran: '5 pelajaran',
          category: 'beginner',
        },
        {
          title: 'React Js',
          description: 'ini adalah decritsncjnd vnfnvjfdnv jenfjwef  cnfvjrlvjm',
          price: 'Rp. 500.000',
          image: require('@/assets/react.jpg'),
          jumlahPelajaran: '5 pelajaran',
          category: 'intermediate',
        },
        {
          title: 'Nuxt Js',
          description: 'ini adalah decritsncjnd vnfnvjfdnv jenfjwef  cnfvjrlvjm',
          price: 'Rp. 200.000',
          image: require('@/assets/nuxt.png'),
          jumlahPelajaran: '5 pelajaran',
          category: 'intermediate',
        },
        {
          title: 'Golang Basic',
          description: 'ini adalah decritsncjnd vnfnvjfdnv jenfjwef  cnfvjrlvjm',
          price: 'free',
          image: require('@/assets/golangweb.png'),
          jumlahPelajaran: '5 pelajaran',
          category: 'beginner',
        },

      ],
      searchQuery: '',
      selectedCategory: 'all',
    }
  },
  methods: {
    updateCategory(category) {
      this.selectedCategory = category;
    },
    handleSearch(event) {
      this.searchQuery = event.target.value;
    },
    updateSearch(value) {
      this.searchQuery = value;
    }
  },
  computed: {
    filteredCourses() {
      let filtered = this.courses;

      if (this.selectedCategory !== 'all') {
        filtered = filtered.filter((item) => {
          return item.category === this.selectedCategory;
        });
      }

      if (this.searchQuery) {
        const sanitizedQuery = this.searchQuery.toLowerCase().replace(/\s+/g, '');
        filtered = filtered.filter((item) => {
          const sanitizedTitle = item.title.toLowerCase().replace(/\s+/g, '');
          return sanitizedTitle.includes(sanitizedQuery);
        });
      }
      return filtered;
    },
  },
}
</script>

<style>
.container-card {
  display: flex;
  justify-content: center;
  background-color: hsl(200, 100%, 15%);
}

.container-card-body {
  justify-content: center;
  margin-top: 10px;
  display: flex;
  flex-wrap: wrap;
  background-color: hsl(200, 100%, 15%);
  padding-bottom: 40px;
}

h5 {
  margin-top: 100px;
  margin-bottom: 100px;
  color: white;
}
</style>