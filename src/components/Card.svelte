<script>
    import Comments from './Comments.svelte';
</script>

<div class="Card">
    <div class="Card-container">
        <div class="Card-header">
            <div class="Card-user">
                <img src="https://i.imgur.com/S6BUwUz.jpg" alt="">
                <h2>
                    ChibiMoon
                    <span>Future, Japon</span>
                </h2>
            </div> 
            <div class="Card-Settings">
                <i class='fas fa-ellipsis-h' />
            </div>
            </div>
        <div class="Card-Photo">
            <figure>
                <img src="https://i.imgur.com/S6BUwUz.jpg" alt="">
            </figure>           
        </div>
        <div class="Card-icons">
            <div class="Card-icon-firts">
                <i class="fas fa heart"/>
                <i class= "fas fa-paper-plane"/>
            </div>
            <div class="Card-icond-second">
                <i class="fas fa-bookmark" />
            </div>
        </div>
            <div class="Card description">
                <h3>ChibiMoon</h3>
                <span>Hola!</span>
            </div>
            <Comments />
    </div>        
</div>    