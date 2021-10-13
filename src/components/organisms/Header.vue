<template>
  <header class="main-header">
    <Container size="80">
      <div class="row">
        <div class="col content">
          <Logo />

          <div class="items">
            <NavBar />
            <SearchForm />
          </div>
        </div>
      </div>
    </Container>
  </header>
</template>

<script>
import { Container } from '@/components/bosons'
import { Logo } from '@/components/atoms'
import { NavBar, SearchForm } from '@/components/molecules'

export default {
  components: { Container, Logo, NavBar, SearchForm }
}
</script>

<style lang="scss" scoped>
.main-header {
  z-index: 2;
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  padding: 1rem 0;
  border-bottom: var(--bor) solid var(--bgc-light-d);
  background-color: var(--bgc-light-l);

  .content {
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    align-items: center;

    .items {
      display: flex;
      flex-flow: row nowrap;
      justify-content: center;
      align-items: center;
    }
  }
}
</style>
