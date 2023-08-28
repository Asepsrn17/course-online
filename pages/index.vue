<template>
  <div class="container-card">
    <div class="container-card-body">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">JavaScript Dasar</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Gratis</h6>
          <b-img class="image-body" thumbnail fluid src="../asset/js2.jpg" alt="Image 1"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content. hghgdvgd
            fdhjfdhgh
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem hic, doloribus eligendi facilis magni
            similique et pariatur laboriosam recusandae dolorem numquam ut nihil? Explicabo dolor tempora obcaecati dicta
            pariatur voluptate?
          </p>
          <div class="card-links">
            <a href="#" class="card-left">70 Pelajaran</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>

      <div class="card">
        <div class="card-body">
          <h5 class="card-title">JavaScript Intermediate</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Gratis</h6>
          <b-img class="image-body" fluid src="../asset/js.jpg" alt="Image 1"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dignissimos quisquam, autem tempore perferendis quae
            possimus minus magni impedit et accusantium, quo cum consequuntur animi necessitatibus fugit earum maxime eum
            magnam.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">100 Pelajaran</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Golang Basic</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Gratis</h6>
          <b-img class="image-body" thumbnail fluid src="https://picsum.photos/250/250/?image=54" alt="Image 1"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">5 Pelajaran</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">React Js</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Gratis</h6>
          <b-img class="image-body" thumbnail fluid src="https://picsum.photos/250/250/?image=54" alt="Image 1"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">11 Pelajaran</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Nuxt Js</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Gratis</h6>
          <b-img class="image-body" thumbnail fluid src="https://picsum.photos/250/250/?image=54" alt="Image 1"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content. Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptate expedita
            magnam ab quae, aliquam est iure corrupti quibusdam deserunt quas? Unde recusandae tenetur dolorum nulla! Quos
            ut vel quis dolor!
          </p>
          <div class="card-links">
            <a href="#" class="card-left">11 Pelajaran</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
</script>

<style>
.card-text {
  margin-top: 10px;
  overflow: hidden;
  text-overflow: ellipsis;
  /* white-space: nowrap; */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 4;
  max-height: 6rem;
  /* line-height: 1.5em; */
  height: 35rem;
}

.image-body {
  width: 100%;
  height: 50%;
}

.container-fluid h3 {
  font-style: italic;
}

.container-card {
  display: flex;
  /* flex-wrap: wrap; */
  justify-content: center;
  background-color: hsl(200, 100%, 15%);
}

.container-card-body {
  justify-content: center;
  margin-top: 40px;
  display: flex;
  flex-wrap: wrap;
  /* justify-content: center; */
  background-color: hsl(200, 100%, 15%);
  padding-bottom: 40px;
}

.card {
  background-color: white;
  /* background-image: url('https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png'); */
  background-size: cover;
  /* Untuk menyesuaikan gambar dengan area */
  background-repeat: no-repeat;
  width: 25rem;
  height: 35rem;
  margin: 50px 10px 30px 10px;
  border: 3px solid hsl(200, 91%, 13%);
  border-radius: 20px;
}

.card-body {
  display: flex;
  flex-direction: column;
  /* justify-content: space-between; */
  flex-grow: 1;
}

.card-links {
  align-items: center;
  display: flex;
  /* justify-content: space-between; */
  margin-top: 10px;
}

.card-left {
  margin-left: 60px;
  color: black;
}

.card-right {
  margin-left: 80px;
}

.card-subtitle {
  font-size: 14px;
}
</style>