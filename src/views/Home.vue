<template>
<div class="home">
  <div class="splash-container">
    <div class="splash">
      <h1 class="splash-head">Hi, my name is Jadon</h1>
    </div>
  </div>

  <div class="content-wrapper">
    <div class="content">
      <h2 class="content-head is-center">I'm an up and coming software developer.</h2>

      <div class="pure-g">
        <div class="l-box pure-u-1 pure-u-md-1-2 pure-u-lg-1-4">

          <h3 class="content-subhead">
            <i class="fa fa-rocket"></i>
            Just Getting Started
          </h3>
          <p>
            I'm a dedicated, fast learner. I have experience with C++, Web Development, and more. And I'm just getting started.
          </p>
        </div>
        <div class="l-box pure-u-1 pure-u-md-1-2 pure-u-lg-1-4">
          <h3 class="content-subhead">
            <i class="fa fa-mobile"></i>
            Mobile Dev
          </h3>
          <p>
            I have a strong interest in mobile development, and I'm working on creating my own mobile apps.
          </p>
        </div>
        <div class="l-box pure-u-1 pure-u-md-1-2 pure-u-lg-1-4">
          <h3 class="content-subhead">
            <i class="fa fa-th-large"></i>
            Projects
          </h3>
          <p>
            I have worked on a number of individual and group projects, within and outside of school.
          </p>
        </div>
        <div class="l-box pure-u-1 pure-u-md-1-2 pure-u-lg-1-4">
          <h3 class="content-subhead">
            <i class="fa fa-check-square-o"></i>
            Certification
          </h3>
          <p>
            I'm in progress to getting a degree in Computer Science, with an emphasis in Software Engineering.
          </p>
        </div>
      </div>
    </div>

    <div class="ribbon l-box-lrg pure-g">
      <div class="l-box-lrg is-center pure-u-1 pure-u-md-1-2 pure-u-lg-2-5">
        <img width="300" alt="Jadon" class="pure-img-responsive" src="../../public/css/layouts/img/jadonsundance.jpg">
      </div>
      <div class=" pure-u-1 pure-u-md-1-2 pure-u-lg-3-5">

        <h2 class="content-head content-head-ribbon">Super cool.</h2>

        <p>
          I'm not really sure what to say here yet... <br>
          But I'll come in and update this later.
          While we are here though, here's the link to my
          <a href="https://github.com/jschol3s/jadon-scholes-home">GitHub Repository</a>
        </p>
      </div>
    </div>
  </div>
</div>
</template>

<style>
.splash-container {
  background-image: url('../../public/css/layouts/img/goldengate.jpg');
  background-size: cover;
  background-position: center;
  background-color: #34495e;
  z-index: 1;
  overflow: hidden;
  width: 100%;
  height: 88%;
  top: 0;
  left: 0;
  position: fixed !important;
}

.splash {
  width: 80%;
  height: 50%;
  margin: auto;
  position: absolute;
  top: 100px;
  left: 0;
  bottom: 0;
  right: 0;
  text-align: center;
  text-transform: uppercase;
}

.splash-head {
  font-size: 20px;
  font-weight: bold;
  color: black;
  border: 3px solid black;
  font-family: "Andale Mono";
  padding: 1em 1.6em;
  font-weight: 100;
  border-radius: 5px;
  line-height: 1em;
}

.splash-subhead {
  color: #424b54;
  font-family: "Andale Mono";
  letter-spacing: 0.05em;
  opacity: 0.8;
}

.content-wrapper {
  position: absolute;
  top: 87%;
  width: 100%;
  min-height: 12%;
  z-index: 2;
  background: white;
}

.content {
  padding: 1em 1em 3em;
}

.content-head {
  font-weight: 400;
  font-family: "Andale Mono";
  text-transform: uppercase;
  letter-spacing: 0.1em;
  margin: 2em 0 1em;
}

.content-head-ribbon {
  color: #d2d0ba;
}

.content-subhead {
  color: #0f5257;
  font-family: "Andale Mono";
}

.content-subhead i {
  margin-right: 7px;
}

.ribbon {
  background: #424b54;
  color: #aaa;
}

body {
  font-family: "Andale Mono";
  font-size: 16px;
}

.home-menu {
  text-align: left;
}

.home-menu ul {
  float: right;
}

.splash {
  width: 50%;
  height: 50%;
}

.splash-head {
  font-family: "Andale Mono";
  font-size: 250%;
}

.l-box-lrg {
  border: none;
}

@media (min-width: 78em) {

  .splash-head {
    font-size: 300%;
    font-family: "Andale Mono";
  }
}
</style>
