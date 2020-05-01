<script>
  export let stories = [];
</script>

<style>
  .Stories {
    border: 1px solid rgba(219, 219, 219, 1);
    border-radius: 5px;
    margin: 1em 0;
    padding: 0.5em 1em;
    background-color: rgba(207, 113, 144, 0.726);
  }
  .Stories-item img {
    width: 40px;
    height: 40px;
    border-radius: 70%;
  }
  .Stories-item {
    display: flex;
    align-items: center;
    margin: 0 1em 0.5em 0;
  }
  .Stories-item h2 {
    font-size: 14px;
    color: rgb(190, 12, 95);
    margin: 0 0 0 1em;
  }
  .Stories-item h2 span {
    display: block;
    font-size: 12px;
    text-transform: uppercase;
    color: white;
  }
  .Stories-head {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.5em 0 0 0;
  }
  .Stories-head h2 {
    font-size: 15px;
    font-weight: 600;
  }
  .Stories-head span {
    font-size: 15px;
    font-weight: normal;
    color: rgb(190, 12, 131);
  }
  .Stories-items {
    margin: 0.5em 0 0.5em 0;
    display: flex;
    justify-content: left;
    align-items: center;
  }
  .Stories-item-box {
    width: 32px;
    height: 32px;
    border: double 2px transparent;
    border-radius: 100%;
    background-image: linear-gradient(#fff, #fff),
      radial-gradient(circle at top left, #f09433, #bc1888);
    background-origin: border-box;
    background-clip: content-box, border-box;
  }
</style>

<div class="Stories">
    <div class="Stories-container">
        <div class="Stories-head">
            <h2>Stories</h2>
            <span> See All</span>
        </div>
        <div class="Stories-items">
        {#each stories as story}
            <div class="Stories-item">
                <div class="Stories-item-box">
                    <img src={story.photo} alt=""/>
                </div>
                <h2>
                    {story.user}
                    <span>{story.hour}</span>
                </h2>
            </div>
        {/each}   
        </div>
    </div>
</div>