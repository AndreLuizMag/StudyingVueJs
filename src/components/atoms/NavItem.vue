<template>
  <a :href="to" class="nav-item">
    {{ content }}
  </a>
</template>

<script>
export default {
  props: {
    content: { type: String, require: true },
    to: { type: String, require: true }
  }
}
</script>

<style lang="scss" scoped>
.nav-item {
  width: fit-content;
  width: -moz-fit-content;
  padding: 0.5rem 1rem;
  display: block;
  font-size: 1.2rem;
  font-weight: bold;
  text-decoration: none;
  line-height: 1;
  color: #4d4a59;
  border-radius: var(--bdr-s);
  transition-duration: var(--tsd);
  transition-property: color, background-color;
  transition-timing-function: var(--ttf);

  &:hover {
    color: var(--blue-dark);
    background-color: var(--blue-light);
  }
}
</style>
