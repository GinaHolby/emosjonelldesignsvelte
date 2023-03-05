<script>
    // CSS //
    import './app.css';

    // Animations //
    import Area from "../animations/Area.svelte";
    import Clickable from "../animations/Clickable.svelte";
    import Important from "../animations/Important.svelte";
    import Noise from "../animations/Noise.svelte";
    import Thinking from "../animations/Thinking.svelte";
    import Wheel from "../animations/Wheel.svelte";

</script>


    <div class="point one">
        <div class="text">
            <h2> 
                Don´t make me think
            </h2>
            <h4>
                Dont make me think by Steve Krug is about how a web page should be design that is as self explanatory as possible.
            </h4>
        </div>
        <div class="animation"> <Thinking/> </div>
    </div>




    <div class="point one">
        <div class="text">
            <h2> 
                Don´t make me think
            </h2>
            <h4>
                Dont make me think by Steve Krug is about how a web page should be design that is as self explanatory as possible.
            </h4>
        </div>
        <div class="animation"> <Wheel/> </div>
    </div>











<style>
   
    .point{
        display: flex;
        gap: 2rem;
        border: pink solid 2px;
        width: 100%;
        min-height: calc(100vh - 4rem);
        align-items: center;
    }
    .text{
        width: 50%;
       /*  display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 1rem; */
    }
    .animation{
        width: 50%;
        

    }
</style>