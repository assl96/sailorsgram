<script>
    import Header from '../components/Header.svelte';
    import Main from '../components/Main.svelte';
    import Sidebar from '../components/Sidebar.svelte';
    import TimeLine from '../components/TimeLine.svelte';
</script>

<style>
    :global(body) {
        background-color: rgb(255, 142, 179);
        color: rgb(41, 51, 182);
    }
</style>

<Header />
<Main>
    <TimeLine />
    <Sidebar />
</Main>