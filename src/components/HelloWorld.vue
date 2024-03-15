<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
  env: Object,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <p>
      You're currently viewing the following environment: <br />
      <b>
        {{ env.VITE_ENV_VARIABLE  }}
      </b>
    </p>
    <p>
      Update #1: Feature request here
    </p>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
