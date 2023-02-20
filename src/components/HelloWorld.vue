<script setup lang="ts">
import { ref } from 'vue'

defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
  <div class="card w-1/3 bg-base-100 shadow-xl">
    <figure><img src="https://evercam.com/wp-content/uploads/sites/11/2019/11/big-red-button.jpg" alt="Red Button" />
    </figure>
    <div class="card-body">
      <h2 class="card-title">{{ msg }}</h2>
      <p>This is a magic button showing how many clicks on it</p>
      <div class="card-actions justify-end">
        <button class="btn btn-primary" @click="count++">count is {{ count }}</button>
      </div>
    </div>
  </div>
</template>
