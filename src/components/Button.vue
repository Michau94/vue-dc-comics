<template>
  <div>
    <span class="button">
      {{ message }}
    </span>
  </div>
</template>

<script>
export default {
  name: "Button",
  props: ["message"],
};
</script>

<style lang="scss" scoped>
@import "../assets/sass/vars.scss";

.button {
  color: white;
  font-weight: bold;
  padding: 8px 30px;
  background-color: $base-color;
}
</style>
