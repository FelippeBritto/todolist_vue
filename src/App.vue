<template>
  <div id="app">
    <section class="hero is-primary is-bold is-fullheight">
      <div class="hero-head">
        <nav class="navbar">
          <div class="container">
            <div class="navbar-brand">
              <a href class="navbar-item">Olá Vue!</a>
            </div>
          </div>
        </nav>
      </div>

      <div class="hero-body">
        <div class="container has-text-centered">
          <div class="row">
            <div class="column">
              <div class="column is-half is-offset-one-quarter">
                <todo-card></todo-card>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="hero-foot">
        <div class="container has-text-centered">
          <div class="content">
            <p>
              <strong>Vue Tutorial</strong> by
              <a href="http://github.com/FelippeBritto">Matheus Brito</a>
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import TodoCard from "./components/TodoCard.vue";

export default {
  name: "app",
  components: {
    TodoCard
  },
  data() {
    return {
      msg: "Hello World!"
    };
  }
};
</script>
<style>
</style>
<scri
