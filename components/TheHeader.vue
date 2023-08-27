<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info" style="height: 120px">
      <b-navbar-nav style="margin-left: 0;">
        <b-nav-item>
          <b-img
            src="~@/static/icon.jpg"
            alt="Ikon"
            width="100"
            height="100"
          ></b-img>
        </b-nav-item>
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

        <b-navbar-nav class="ml-auto">
          <b-nav-form>
            <b-form-input
              size="sm"
              class="mr-sm-2"
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