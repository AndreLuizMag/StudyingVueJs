<template>
  <a :href="to" class="link" target="_blank" rel="noopener noreferrer">
    <img :src="iconPath" :alt="name" />
  </a>
</template>

<script>
export default {
  props: {
    name: { Type: String, require: true },
    icon: { Type: String, require: true },
    to: { Type: String, require: true }
  },
  computed: {
    iconPath() {
      return require(`@/assets/image/icon/${this.icon}.svg`)
    }
  }
}
</script>

<style lang="scss" scoped>
.link {
  width: fit-content;
  width: -moz-fit-content;
  display: flex;
  padding: 0.75rem;
  border-radius: 4px;
  transition-duration: var(--tsd);
  transition-property: background-color;
  transition-timing-function: var(--ttf);

  img {
    transition-duration: var(--tsd);
    transition-property: transform;
    transition-timing-function: var(--ttf);
  }

  &:hover {
    background-color: var(--blue-light);
  }

  &:focus {
    img {
      transform: scale(0.9);
    }
  }
}
</style>
