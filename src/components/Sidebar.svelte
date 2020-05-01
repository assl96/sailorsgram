<script>
    import Stories from './Stories.svelte'
    import Footer from './Footer.svelte'

    export let stories;

</script>

<style>
  .Sidebar {
    padding: 4.5em 0 0 0;
  }

</style>

<div class="Sidebar">
    <div class="Sidebar-container">
        <Stories {stories}/>
        <Footer />
    </div>
</div>