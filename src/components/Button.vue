<template>
  <button :style="{ background: buttonColor }" class="btn " @click="onClick()">
    {{ buttonText }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    buttonText: String,
    buttonColor: String,
  },
  methods: {
    onClick() {
      this.$emit("toggle-add-task");
    },
  },
};
</script>

<style scoped></style>
