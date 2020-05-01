<script>
    import Profile from './Profile.svelte'
    import Stories from './Stories.svelte'
    import Footer from './Footer.svelte'


    export let nickname;
    export let name;
    export let stories;

</script>

<style>
  .Sidebar {
    padding: 4.5em 0 0 0;
  }
  .Sidebar-container {
 
  }
</style>

<div class="Sidebar">
    <div class="Sidebar-container">
        <Profile {nickname} {name}/>
        <Stories {stories}/>
        <Footer />
    </div>
</div>