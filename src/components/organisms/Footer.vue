<template>
  <footer class="main-footer">
    <Container size="80">
      <div class="row">
        <div class="col">
          <SocialNetwork />
        </div>
      </div>
    </Container>
  </footer>
</template>

<script>
import { SocialNetwork } from '@/components/molecules'

export default {
  components: {
    SocialNetwork
  }
}
</script>

<style lang="scss" scoped>
.main-footer {
  width: 100%;
  border-top: var(--bor) solid var(--bgc-light-d);
  padding: 2rem 0;
}
</style>
