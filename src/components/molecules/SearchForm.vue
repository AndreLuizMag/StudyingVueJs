<template>
  <div class="search-bar">
    <input type="search" name="search" id="search" placeholder="Pesquisar" />
    <div class="icon">
      <svg
        width="25"
        height="25"
        viewBox="0 0 25 25"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M11.014 19.1559C15.4323 19.1559 19.014 15.5742 19.014 11.1559C19.014 6.73761 15.4323 3.15588 11.014 3.15588C6.59576 3.15588 3.01404 6.73761 3.01404 11.1559C3.01404 15.5742 6.59576 19.1559 11.014 19.1559Z"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M21.014 21.1559L16.664 16.8059"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.search-bar {
  position: relative;
  border-radius: 4px;
  overflow: hidden;

  input {
    width: 100%;
    padding: 0.75rem 1rem 0.75rem calc(1rem + 25px);
    border: 2px solid #f4f4f4;
    outline: 0;
    transition-duration: 0.25s;
    transition-property: box-shadow;
    transition-timing-function: ease-in;

    &:focus,
    &:focus-visible {
      box-shadow: inset 0px 0px 0px 2px #e7eefe;
    }
  }

  .icon {
    position: absolute;
    bottom: 0.25rem;
    left: 0.5rem;

    svg {
      path {
        stroke: #4d4a59;
      }
    }
  }

  &::before {
    content: '';
    width: 100%;
    height: 2px;
    position: absolute;
    bottom: 0;
    left: 0;
    background-color: #86acf9;
  }

  &:focus {
    &::before {
      background-color: red;
    }
  }
}
</style>
