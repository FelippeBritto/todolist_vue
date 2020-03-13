<template>
  <div class="row">
    <div class="columns">
      <div class="column is-half is-offset-one-quarter">
        <div class="field is-grouped">
          <p class="control is-expanded">
            <input
              class="input is-primary has-text-centered"
              type="text"
              placeholder="Nova tarefa..."
              v-model="tarefa"
            />
          </p>
          <p class="control">
            <a class="button is-success add-button">
              <span class="icon is-small">
                <i class="fa fa-plus"></i>
              </span>
            </a>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "novo-todo",
  data() {
    return {
      tarefa: ""
    };
  }
};
</script>
<style scoped>
</style>
