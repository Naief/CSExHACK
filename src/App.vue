<template>
  <div class="cat-container container-fluid">
    <div class="cat-navbar row navbar navbar-expand-sm sticky-top" role="navigation">
      <div class="collapse navbar-collapse" id="navigationToggle">
        <div class="col-sm-1">
          <router-link class="cat-navbar-text" to="/">Home</router-link>
        </div>
        <!-- <div class="col-sm-1">
          <router-link class="cat-navbar-text" to="/cases">Cases</router-link>
        </div>-->
        <div class="col-sm-1">
          <router-link class="cat-navbar-text" to="/faq">FAQ</router-link>
        </div>
        <!-- <div class="col-sm-1">
          <router-link class="cat-navbar-text" to="/about">About</router-link>
        </div>-->
        <div class="col-sm-1">
          <router-link class="cat-navbar-text" to="/terms">Terms</router-link>
        </div>
      </div>
    </div>

    <!-- content goes here -->
    <div class="cat-content row">
      <router-view/>
    </div>
    <!-- ------------------ -->

    <div class="cat-footer container-fluid">
      <div class="cat-info row">
        <div class="cat-contact col-sm-3">
          <h3>Contact</h3>
          <ul>
            <li>
              <a v-bind:href="cat_data.facebook" target="_blank">Facebook</a>
            </li>
            <li>
              <a v-bind:href="cat_data.twitter" target="_blank">Twitter</a>
            </li>
            <li>
              Email
              <a v-bind:href="cat_data.mail">cat@gota.gu.se</a>
            </li>
          </ul>
        </div>
        <div class="cat-location col-sm-3">
          <h3>Location</h3>
          <ul>
            <li>
              <a v-bind:href="cat_data.location" target="_blank">Forskningsgången 6, 417 56 Göteborg</a>
            </li>
          </ul>
        </div>
        <div class="cat-signup col-sm-3">
          <h3>Become a member of Ctrl-Alt-Team</h3>
          <ul>
            <li>
              click
              <a v-bind:href="cat_data.signup">here</a>
            </li>
          </ul>
        </div>
        <div class="cat-gu col-sm-3">
          <h3>Interested in Gothenburg University's Computer Science Department?</h3>
          <ul>
            <li>
              Click
              <a v-bind:href="cat_data.gu" target="_blank">here</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="cat-legal row">
        <div class="col-sm-3">
          <p>Copyright &copy; 2019 CTRL-Alt-TEAM. All rights reserved.</p>
        </div>
        <div class="col-sm-3">
          <p>Made with ❤️ by C.A.T.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import cat_data from "@/assets/values/links.js";
export default {
  name: "App",
  data() {
    return {
      cat_data: cat_data
    };
  }
};
</script>

<style>
/* general */
.cat-container {
  background-color: black;
  position: relative;
  min-height: 100vh;
}
/* navbar */
@import url("https://fonts.googleapis.com/css?family=Inconsolata");
.cat-navbar {
  text-align: center;
  background-color: black;
}
.cat-navbar-text {
  color: white;
  text-decoration: none;
  font-family: "Inconsolata", monospace;
  font-size: 1.5em;
  font-weight: bold;
}

/* content */
.cat-content {
  position: inherit;
  height: 100%;
  /* pad the bottom with the height of the footer. its a patch solution, but a begger should never be picky ;( */
  padding-bottom: 25vh;
}

/* footer */
@import url("https://fonts.googleapis.com/css?family=Inconsolata");
.cat-footer {
  background-color: black;
  color: white;
  text-decoration: none;
  font-family: "Inconsolata", monospace;
  font-size: 1em;
  padding-top: 2vh;

  /* since the container in the app component is set to the height of the screen,
we position the footer at the bottom of the page absolute to the container that the footer is in.
in other words, footer is inside another container that has the height of the entire screen and
a relative position 
source: https://medium.freecodecamp.org/how-to-keep-your-footer-where-it-belongs-59c6aa05c59c */
  position: absolute;
  height: 25vh;
  bottom: 0;
  left: 0;
}
.cat-footer h3 {
  font-size: 1.2em;
}
.cat-contact h3 {
  color: white;
}
.cat-location h3 {
  color: green;
}
.cat-signup h3 {
  color: yellow;
}
.cat-gu h3 {
  color: blueviolet;
}
.cat-legal {
  font-size: 0.8em;
}
</style>
