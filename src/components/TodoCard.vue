<template>
  <div class="card">
    <header class="card-header">
      <p class="card-header-title has-text-left">{{hoje}}</p>
      <div class="has-text-right">
        <p class="card-header-title">{{tarefas.length}} tarefas</p>
      </div>
    </header>
    <div class="card-content">
      <div class="content"></div>
      <div class="content"></div>
    </div>
  </div>
</template>

<script>
import NovoTodo from "./NovoTodo";
export default {
  name: "todo-card",
  components: {
    NovoTodo
  },
  data() {
    return {
      dias: [
        "Domingo",
        "Segunda",
        "Ter?a",
        "Quarta",
        "Quinta",
        "Sexta",
        "S?bado"
      ],
      meses: [
        "Janeiro",
        "Fevereiro",
        "Marco",
        "Abril",
        "Maio",
        "Junho",
        "Julho",
        "Agosto",
        "Setembro",
        "Outubro",
        "Novembro",
        "Dezembro"
      ],
      tarefas: []
    };
  },
  computed: {
    hoje: function() {
      let novaData = new Date();
      return `${(this.dias = [novaData.getDay()])}, ${novaData.getDate()} de ${
        this.meses[novaData.getMonth()]
      }`;
    }
  }
};
</script>
<style>
.card {
  border-radius: 10px;
}
.card-header-title {
  color: #636368;
}
</style>
