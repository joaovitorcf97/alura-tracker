<template>
  <div class="box">
    <div class="columns">
      <div
        class="column is-8"
        role="form"
        atia-label="Formlario de uma criação para uma nova tarefe"
      >
        <input
          type="text"
          class="input"
          placeholder="Qual tarefa você deseja iniciar?"
        />
      </div>
      <div class="column">
        <div
          class="is-flex is-align-items-center is-justify-content-space-between"
        >
          <section>
            <strong>00:00:00</strong>
          </section>
          <button class="button" @click="iniciar">
            <span class="icon">
              <i class="fas fa-play"></i>
            </span>
            <span>play</span>
          </button>
          <button class="button" @click="finalizar">
            <span class="icon">
              <i class="fas fa-stop"></i>
            </span>
            <span>stop</span>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "FormularioComponent",
  methods: {
    iniciar() {
      console.log("Iniciando");
    },
    finalizar() {
      console.log("Finalizando");
    },
  },
});
</script>

<style scoped>
</style>