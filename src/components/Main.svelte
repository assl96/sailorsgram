<style>
  .Main {
    display: grid;
    grid-template-columns: minmax(auto, 936px);
    justify-content: center;
  }
  .Main-container {
    display: grid;
    grid-template-columns: 1fr;
    grid-gap: 0.0000001em;
    padding: 2em 0;
  }
</style>

<div class="Main">
    <div class="Main-container">
    <slot />
    </div>
</div>