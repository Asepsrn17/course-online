<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info" style="height: 120px">
      <b-navbar-nav>
        <b-col md="6" class="mb-3">
        <b-icon icon="star-fill" animation="fade" font-scale="4"></b-icon>
    </b-col>
      </b-navbar-nav>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav style="margin-left: 50px">
        <b-navbar-nav style="margin: 10px 0 10px 0">
          <b-nav-item-dropdown center>
            <template #button-content>
              <em class="user-text">Daftar Kursus</em>
            </template>
            <b-dropdown-item href="#">JavaScript</b-dropdown-item>
            <b-dropdown-item href="#">Golang</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown center>
            <template #button-content>
              <em class="user-text">Kategori</em>
            </template>
            <b-dropdown-item href="#">Beginner</b-dropdown-item>
            <b-dropdown-item href="#">Intermediate</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>

        <b-navbar-nav class="ml-auto" style="margin-right: 400px;">
          <b-nav-form>
            <b-form-input
              size="sm"
              class="mr-lg-2"
              placeholder="Search"
            ></b-form-input>
            <b-button size="sm" class="my-2 my-sm-0" type="submit"
              >Search</b-button
            >
          </b-nav-form>
        </b-navbar-nav>
      </b-collapse>
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
}
</script>

<style>
.user-text {
  font-weight: bold;
  font-size: 16px;
  color: #fff;
  margin-left: 30px;
}
.user-text:hover {
  font-size: 18px;
}
</style>