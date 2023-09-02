<template>
  <div class="container-card">
    <div class="container-card-body">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">JavaScript Dasar</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Gratis</h6>
          <b-img class="image-body" thumbnail fluid src="~/assets/jsdasar.jpg" alt="javascript"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content. hghgdvgd
            fdhjfdhgh
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quidem hic, doloribus eligendi facilis magni
            similique et pariatur laboriosam recusandae dolorem numquam ut nihil? Explicabo dolor tempora obcaecati dicta
            pariatur voluptate?
          </p>
        </div>
        <div class="card-links">
          <p class="card-left">5 Pelajaran</p>
          <p class="card-right">5 Pelajaran</p>
        </div>
        <div class="button-container">
          <b-button block variant="primary" class="button-card">Selengkapnya</b-button>
        </div>
      </div>

      <div class="card">
        <div class="card-body">
          <h5 class="card-title">JavaScript Intermediate</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Rp.200.000</h6>
          <b-img class="image-body" fluid src="~/assets/jsdasar.jpg" alt="javascript"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dignissimos quisquam, autem tempore perferendis quae
            possimus minus magni impedit et accusantium, quo cum consequuntur animi necessitatibus fugit earum maxime eum
            magnam.
          </p>
        </div>
        <div class="card-links">
          <p class="card-left">100 Pelajaran</p>
          <p class="card-right">Mulai belajar</p>
        </div>
        <div class="button-container">
          <b-button block variant="primary" class="button-card">Selengkapnya</b-button>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Golang Basic</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Gratis</h6>
          <b-img class="image-body" thumbnail fluid src="~/assets/golangweb.png" alt="Golang"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
        </div>
        <div class="card-links">
          <p class="card-left">5 Pelajaran</p>
          <p class="card-right">Mulai belajar</p>
        </div>
        <div class="button-container">
          <b-button block variant="primary" class="button-card">Selengkapnya</b-button>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">React Js</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Rp.300.000</h6>
          <b-img class="image-body" thumbnail fluid src="~/assets/react.jpg" alt="react"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
        </div>
        <div class="card-links">
          <p class="card-left">50 Pelajaran</p>
          <p class="card-right">Mulai belajar</p>
        </div>
        <div class="button-container">
          <b-button block variant="primary" class="button-card">Selengkapnya</b-button>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Nuxt Js</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Gratis</h6>
          <b-img class="image-body" thumbnail fluid src="~/assets/nuxt.png" alt="nuxt"></b-img>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content. Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptate expedita
            magnam ab quae, aliquam est iure corrupti quibusdam deserunt quas? Unde recusandae tenetur dolorum nulla! Quos
            ut vel quis dolor!
          </p>
        </div>
        <div class="card-links">
          <p class="card-left">11 Pelajaran</p>
          <p class="card-right">Mulai belajar</p>
        </div>
        <div class="button-container">
          <b-button block variant="primary" class="button-card">Selengkapnya</b-button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
</script>

<style>
.button-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 10px;
  width: 80%;
}

.button-container {
  margin-top: auto;
  width: 400px;
  display: flex;
  justify-content: center;
  padding-bottom: 10px;
}

.card-text {
  margin-top: 10px;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 4;
  max-height: 6rem;
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
  justify-content: center;
  background-color: hsl(200, 100%, 15%);
}

.container-card-body {
  justify-content: center;
  margin-top: 40px;
  display: flex;
  flex-wrap: wrap;
  background-color: hsl(200, 100%, 15%);
  padding-bottom: 40px;
}

.card {
  background-color: white;
  background-size: cover;
  background-repeat: no-repeat;
  width: 25rem;
  height: 35rem;
  margin: 50px 10px 30px 10px;
  border: 3px double hsl(200, 91%, 13%);
  border-radius: 10px;
}

.card-body {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
}

.card-links {
  display: flex;
  justify-content: center;
  display: flex;
  margin-bottom: 10px;
}

.card-left {
  background-color: rgba(0, 0, 0, 0.6);
  color: white;
  font-weight: bold;
  font-size: 12px;
  padding: 5px 5px;
  margin-right: 40px;
}

.card-right {
  background-color: rgba(0, 0, 0, 0.6);
  color: white;
  font-weight: bold;
  font-size: 12px;
  padding: 5px 5px;
  margin-left: 40px;
}

.card-title {
  font-weight: bold;
}

.card-subtitle {
  font-size: 14px;
  color: red;
  font-style: italic;
  margin-top: 5px;
  font-weight: bold;
  font-family: Arial, Helvetica, sans-serif;
}
</style>