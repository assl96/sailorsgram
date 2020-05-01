<script>
    import { onMount } from "svelte";
    import Header from '../components/Header.svelte';
    import Main from '../components/Main.svelte';
    import Sidebar from '../components/Sidebar.svelte';
    import TimeLine from '../components/TimeLine.svelte';
    import {Api} from '../api.js'

    let data = Api;
    // const Api = "https://us-central1-pugstagram-co.cloudfunctions.net/data";

    onMount(async () => {
        // const response = await fetch(Api)
        // data = await response.json()
    });

</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Lato:wght@300;400;700&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Pacifico&display=swap');
    :global(body) {
        background-color: rgb(255, 142, 179);
        color: rgb(255, 255, 255);
        font-family: 'Lato', sans-serif;
        margin: 0;
        padding: 0;
    }

    :global(h1,h2,h3){
        margin: 0;
        padding: 0;
    }
    
</style>

<Header />
<Main>
    <Sidebar {...data.user} stories={data.stories}/>
    <TimeLine posts={data.posts} />
</Main>