<template>
  <div class="app-bar">
    <span class="app-bar-l" @click="$emit('left')">
      <i :class="['fa', `fa-${left}`]"></i>
    </span>
    <h1>{{title}}</h1>
    <span class="app-bar-r" @click="$emit('right')">
      <i :class="['fa', `fa-${right}`]"></i>
    </span>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: "",
    },
    left: {
      type: String,
      default: "chevron-left",
    },
    right: {
      type: String,
      default: "ellipsis-v",
    },
  },
};
</script>

<style>
</style>