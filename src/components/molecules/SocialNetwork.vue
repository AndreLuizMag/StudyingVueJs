<template>
  <div class="social-network">
    <SocialLink
      name="Github"
      to="https://github.com/AndreLuizMag"
      icon="github"
    />
    <SocialLink
      name="Codepen"
      to="https://codepen.io/AndreLuizMag"
      icon="codepen"
    />
  </div>
</template>

<script>
import { SocialLink } from '@/components/atoms'

export default {
  components: { SocialLink }
}
</script>

<style lang="scss" scoped>
.social-network {
  width: fit-content;
  width: -moz-fit-content;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-around;
  align-items: center;
  gap: 0.5rem;
}
</style>
