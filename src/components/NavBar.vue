<template>
    <b-navbar toggleable="lg" type="light" variant="light" fixed="top" sticky="true" class="shadow-sm rounded">
      <b-navbar-brand to="/">
        <img src="@/assets/img/logohimatika.png" fluid alt="hima logo" width="180px" height="auto">
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item to="/">Home</b-nav-item>
          <b-nav-item to="/">Acara</b-nav-item>
          <b-nav-item to="/about">Tentang</b-nav-item>
          
          <!-- dropdown -->
          <b-nav-item-dropdown text="More" right>
            <b-dropdown-item href="#">Visi & Misi</b-dropdown-item>
            <b-dropdown-item href="#">Struktur Oraganisai</b-dropdown-item>
            <b-dropdown-item href="#">Kontak Kami</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
</template>

<script>
export default {
    name: "NavBar"
}
</script>