<template>
<div>
  <div class="header">
    <div class="home-menu pure-menu pure-menu-horizontal pure-menu-fixed">
      <a class="pure-menu-heading" href="">JS</a>

      <ul class="pure-menu-list">
        <li class="pure-menu-item">
          <router-link to="/" class="pure-menu-link">Home</router-link>
        </li>
        <li class="pure-menu-item">
          <router-link to="/about" class="pure-menu-link">About</router-link>
        </li>
        <li class="pure-menu-item">
          <router-link to="/contact" class="pure-menu-link">Contact Me</router-link>
        </li>
        <li class="pure-menu-item"><a href="/JadonNewResume.pdf" class="pure-menu-link">Resume</a></li>
        <li class="pure-menu-item"><a href="https://www.linkedin.com/in/jadon-scholes-a97110172/" class="pure-menu-link">LinkedIn</a></li>
      </ul>
    </div>
  </div>
  <div class="content">
    <router-view />
  </div>
</div>
</template>

<style>
.home-menu {
  padding: 0.5em;
  text-align: left;
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.10);
}

.home-menu {
  background: #424b54;
}

.pure-menu.pure-menu-fixed {
  /* Fixed menus normally have a border at the bottom. */
  border-bottom: none;
  /* I need a higher z-index here because of the scroll-over effect. */
  z-index: 4;
}

.home-menu .pure-menu-heading {
  color: #d2d0ba;
  font-weight: 400;
  font-size: 120%;
}

.home-menu .pure-menu-selected a {
  color: #93a8ac;
}

.home-menu a {
  color: #d2d0ba;
}

.home-menu li a:hover,
.home-menu li a:focus {
  background: none;
  border: none;
  color: #93a8ac;
}
</style>
