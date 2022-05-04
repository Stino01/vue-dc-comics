<template>
  <main>
    <div class="container">
      <p>Content goes here</p>
    </div>
  </main>
</template>

<script>
export default {
  name: 'AppMain',
}
</script>

<style lang="scss">
  @import "../style/variables.scss";

  main {
    background-color: $bg-black;

    .container {
      @include my-container;
      color: white;
      padding: 3em 0;

      p {
        font-size: 22px;
      }
    }
  }
</style>