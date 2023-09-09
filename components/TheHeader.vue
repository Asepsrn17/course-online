<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info" style="height: 140px;">
      <b-navbar-nav>
        <b-col md="6" class="mb-3">
          <b-icon icon="star-fill" animation="fade" font-scale="4"></b-icon>
        </b-col>
      </b-navbar-nav>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav style="padding-left: 50px; z-index: 1000;">
        <b-navbar-nav style="margin: 10px 0 10px 0">
          <b-nav-item-dropdown center>
            <template #button-content>
              <em class="user-text">Informasi</em>
            </template>
            <b-dropdown-item href="about">Tentang Course</b-dropdown-item>
            <b-dropdown-item href="blog">Blog</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown center>
            <template #button-content>
              <em class="user-text">Kategori</em>
            </template>
            <b-dropdown-item @click="updateCategory('all')">Semua</b-dropdown-item>
            <b-dropdown-item @click="updateCategory('beginner')">Beginner</b-dropdown-item>
            <b-dropdown-item @click="updateCategory('intermediate')">Intermediate</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>

        <b-navbar-nav class="ml-auto">
          <b-nav-form class="mr-5">
            <b-form-input size="sm" class="mr-lg-2" v-model="searchQuery" @input="updateSearchQuery"
              placeholder="apa yang ingin dipelajari ?" style="width: 400px;">
            </b-form-input>
          </b-nav-form>
        </b-navbar-nav>
      </b-collapse>
      <div class="mr-4">
        <b-button href="register" pill class="mr-3">Daftar</b-button>
        <b-button href="login" pill variant="primary">Masuk</b-button>
      </div>
    </b-navbar>
  </div>
</template>

<script>
import { BIcon, BIconArrowUp, BIconArrowDown } from 'bootstrap-vue'

export default {
  components: {
    BIcon,
    BIconArrowUp,
    BIconArrowDown
  },
  props: {
    searchQuery: String
  },
  methods: {
    submitSearch() {
      this.$emit('search', this.searchQuery);
    },
    updateSearchQuery(value) {
      this.$emit('update-search', value)
    },
    updateCategory(value) {
      this.$emit('category', value)
    }
  }
}
</script>

<style>
b-nav-item-dropdown:hover {
  background-color: white;
}

.user-text {
  font-weight: bold;
  font-size: 16px;
  color: #fff;
  margin-left: 30px;
}

.user-text-login {
  font-weight: bold;
  font-size: 14px;
  color: #fff;
  padding-left: 6px;
}

.user-text-login:hover {
  font-weight: bold;
  font-size: medium;
}

.user-text:hover {
  font-size: 18px;
}
</style>