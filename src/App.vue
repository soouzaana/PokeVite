<script setup>
import { ref } from "vue";

let num = ref(0);
</script>

<template>
  <div>
    <!--NAVBAR-->
    <nav class="navbar navbar-expand-lg navbar-dark theme-pink">
      <div class="container-fluid">
        <router-link class="navbar-brand" to="/">
          <img
            src="https://cdn-icons-png.flaticon.com/512/188/188987.png"
            alt="Logo"
            width="30"
            height="24"
            class="d-inline-block align-text-top"
          />
          PokeVite
        </router-link>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <router-link class="nav-link" aria-current="page" to="/"
                >Home</router-link
              >
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/about">About</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!--CONTENT-->
    <div class="main">
      <router-view></router-view>
    </div>

    <!--FOOTER-->
    <footer class="theme-pink text-light">
      <div>Design in {{ new Date().getFullYear() }}</div>
    </footer>
  </div>
</template>

<style>
body {
  background: rgb(249, 179, 211);
  background: linear-gradient(
    0deg,
    rgba(249, 179, 211, 1) 0%,
    rgba(245, 124, 153, 1) 100%
  );
  height: 100vh;
}

footer {
  align-items: center;
  bottom: 0;
  display: flex;
  height: 56px;
  justify-content: center;
  position: fixed;
  width: 100%;
}

.theme-pink {
  background-color: #f05eaf;
}
</style>
