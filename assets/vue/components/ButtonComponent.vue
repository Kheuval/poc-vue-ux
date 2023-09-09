<template>
  <button :class="classNames" @click="log">{{ text }}</button>
</template>

<script lang="ts" setup>
defineProps<{
  text: string,
  classNames: string | string[],
}>();

const log = () => {
  console.log("It works !");
}
</script>
