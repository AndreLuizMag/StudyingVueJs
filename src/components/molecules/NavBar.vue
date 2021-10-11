<template>
  <nav class="nav-bar">
    <NavItem content="Home" to="/home" />
    <NavItem content="About" to="/about" />
    <NavItem content="Contact" to="/contact" />
  </nav>
</template>

<script>
import { NavItem } from '@/components/atoms'

export default {
  components: { NavItem }
}
</script>

<style lang="scss" scoped>
.nav-bar {
  width: 100%;
  display: flex;
  flex-flow: row nowrap;
  justify-content: center;
  align-items: center;
  gap: 1rem;
}
</style>
