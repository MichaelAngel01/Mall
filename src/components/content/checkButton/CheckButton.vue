<template>
  <div class="check-button" :class="{ check: IsCheck }">
    <img src="~assets/img/cart/tick.svg" />
  </div>
</template>
<script>
export default {
  name: "CheckButton",
  props: {
    IsCheck: {
      type: Boolean,
      default: false,
    },
  },
};
</script>
<style scoped>
.check-button {
  position: relative;
  margin: 0;
  width: 18px;
  height: 18px;
  border-radius: 50%;
  border: 2px solid #ccc;
  cursor: pointer;
}
.check {
  background-color: var(--color-tint);
  border-color: var(--color-tint);
}
</style>
