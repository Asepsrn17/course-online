<template>
    <div class="card">
        <div class="card-body">
            <h4 class="card-title">{{ course.title }}</h4>
            <h6 class="card-subtitle mb-3 text-body-secondary">{{ course.price }}</h6>
            <b-img class="image-body" thumbnail fluid :src="course.image"></b-img>
            <p class="card-text">
                {{ course.description }}
            </p>
        </div>
        <div class="card-links">
            <p class="card-left">{{ course.jumlahPelajaran }}</p>
            <p class="card-right"> {{ course.category }}</p>
        </div>
        <div class="button-container">
            <b-button block variant="primary" class="button-card">Selengkapnya</b-button>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        course: {
            type: Object,
            default: 'untitled'
        }
    }
}
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