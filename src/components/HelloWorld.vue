<template>
  <div>
    <p>{{ message }}</p>
    <button @click="updateMessage">Update Message</button>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";

const message = ref("Hello, Vue!");

const updateMessage = () => {
  message.value = "Hello, Vue updated!";
};
</script>
