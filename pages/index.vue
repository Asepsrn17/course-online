<template>
  <div class="container-card">
    <div class="container-card-body">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">JavaScript Dasar</h5>
          <h6 class="card-subtitle mb-3 text-body-secondary">Gratis</h6>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">Silabus</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">JavaScript Intermediate</h5>
          <h6 class="card-subtitle mb-2 text-body-secondary">Gratis</h6>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">Silabus</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Golang Basic</h5>
          <h6 class="card-subtitle mb-2 text-body-secondary">Gratis</h6>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">Silabus</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Java</h5>
          <h6 class="card-subtitle mb-2 text-body-secondary">Gratis</h6>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">Silabus</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">Flutter</h5>
          <h6 class="card-subtitle mb-2 text-body-secondary">Gratis</h6>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">Silabus</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">MySql</h5>
          <h6 class="card-subtitle mb-2 text-body-secondary">Gratis</h6>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">Silabus</a>
            <a href="#" class="card-right">Mulai belajar</a>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card-body">
          <h5 class="card-title">MySql</h5>
          <h6 class="card-subtitle mb-2 text-body-secondary">Gratis</h6>
          <p class="card-text">
            Some quick example text to build on the card title and make up the
            bulk of the card's content.
          </p>
          <div class="card-links">
            <a href="#" class="card-left">Silabus</a>
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
.container-fluid h3 {
  font-style: italic;
}
.container-card {
  display: flex;
  /* flex-wrap: wrap; */
  /* justify-content: center; */
  background-color: hsl(200, 100%, 15%);
}
.container-card-body {
  margin-top: 50px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  background-color: hsl(200, 100%, 15%);
  padding-bottom: 40px;
}

.card {
  background-color: white;
  /* background-image: url('https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png'); */
  background-size: cover; /* Untuk menyesuaikan gambar dengan area */
  background-repeat: no-repeat;
  width: 18rem;
  height: 28rem;
  margin: 20px 10px 30px 10px;
  border: 3px solid #17a2b8;
  border-radius: 20px;
}

.card-body {
  display: flex;
  flex-direction: column;
  /* justify-content: space-between; */
  flex-grow: 1;
}

.card-links {
  display: inline-block;
  flex-direction: column;
  margin-top: 130px;
}
.card-left {
  margin-left: 20px;
  color: black fons;
}
.card-right {
  margin-left: 50px;
}

.card-subtitle {
  margin-top: 25px;
}
</style>