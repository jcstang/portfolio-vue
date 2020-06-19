<template>
  <section class="header-section columns">
    <div class="col-md-3 column is-one-third-desktop">
      <img class="align-self-start mr-3" :src="meImage" alt="Jacob Stanger portrait" />
    </div>
    <div class="col-md-9 column">
      <h5 class="title is-2">Jacob Stanger</h5>
      <h5 class="title is-3">About Me</h5>
      <p>
        Full stack web developer with a passion for iOS development. Educated in
        computer science at Weber State University and recently earned a coding
        certificate from the University of Utah. Life-long learner that thrives
        in team environments and is driven by complex problem solving with more
        than 100 hours on Udemy and Pluralsight. Expertise interfacing and
        scoping solutions with clients and clearly explaining technical topics
        to stakeholders.
      </p>
      <hr />
      <p>
        <strong>Email</strong> JacobcStanger@gmail.com
      </p>
      <div class="row container is-fluid">
        <a
          class="button is-link social-btn"
          href="https://www.linkedin.com/in/jacob-stanger/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <span class="icon">
            <i class="fab fa-linkedin"></i>
          </span>
          <span>LinkedIn</span>
        </a>

        <a
          class="button is-link social-btn"
          href="https://github.com/jcstang"
          target="_blank"
          rel="noopener noreferrer"
        >
          <span class="icon">
            <i class="fab fa-github"></i>
          </span>
          <span>GitHub</span>
        </a>

        <a
          class="button is-info social-btn"
          href="https://twitter.com/jc_stang"
          target="_blank"
          rel="noopener noreferrer"
        >
          <span class="icon">
            <i class="fab fa-twitter"></i>
          </span>
          <span>Twitter</span>
        </a>
        <div class="container">
          <img
            src="../../public/badge-coding-bootcamp-trilogy.png"
            alt="developer certificate"
            class="badge-img"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import "bulma/css/bulma.css";

export default {
  name: "Header",
  props: {
    msg: String,
    meImage: String
  }
};
</script>

<style scoped>
.header-section {
  padding-top: 1rem;
  padding-bottom: 1rem;
  margin-bottom: 2rem;
}

.social-btn {
  margin-bottom: 1rem;
  margin-right: 1rem;
}

.badge-img {
  max-width: 12vw;
}
</style>
