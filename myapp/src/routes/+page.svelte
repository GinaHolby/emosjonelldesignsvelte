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
    import Smily from "../animations/Smily.svelte";
    import Smilyy from "../animations/Smilyy.svelte"


    

    


    let correctClick = true

 



</script>







    <div class="point hero">
        <div class="text">
            <h1> 
                Don´t make me think
            </h1>
            <h3>
                Dont make me think by Steve Krug is about how a web page should be design that is as self explanatory as possible.
            </h3>
            <h3>He describes several princepals in his book that makes a website easy to understand and use. 
            </h3>
        </div>
        <div class="animation" > <Thinking/> </div>
    </div>





    <div class="point one">
        <div class="animation"> <Wheel/> </div>
        <div class="text">
            <h3> 
                Don´t reinvent the wheel, use conventions
            </h3>
            <h4> Quote: </h4>
            <h4> <i> 
                All conventions start life as somebody’s bright idea. If the idea works well enough, other sites imitate it and eventually enough people have seen it in enough places that it needs no explanation. This adoption process takes time, but it happens pretty quickly on the Internet, like everything else. For instance, enough people are now familiar with the convention of using a metaphorical shopping cart on e-commerce sites that it’s safe for designers to use a shopping cart icon without labeling it “Shopping cart.”
            </i>
            </h4>
        </div>
       
       
    </div>



    

    <div class="point one">
        <div class="text">
            <h3> 
                Break up pages into clearly defined areas
            </h3>
            <h4> Quote: </h4>
            <h4> <i> 
                Dividing the page into clearly defined areas is important because it allows users to decide quickly which areas of the page to focus on and which areas they can safely ignore. Several of the initial eye-tracking studies of Web page scanning suggest that users decide very quickly which parts of the page are likely to have useful information and then almost never look at the other parts—almost as though they weren’t there.            </i>
            </h4>
        </div>
        <div class="animation"> <Area/> </div>
       
    </div>

    <div class="point one">
        <div class="animation"> <Clickable/> </div>
        <div class="text">
            <h3> 
                Make it obvious what's clickable
            </h3>
            <h4> Quote: </h4>
            <h4> <i> 
                Since a large part of what people are doing on the Web is looking for the next thing to click, it’s important to make it obvious what’s clickable and what’s not.
            </i></h4>
        </div>
        
       
    </div>

    <div class="point one">
        <div class="text">
            <h3> 
                Create a Visual hierarchy 
            </h3>
            <h4> Quote: </h4>
            <h4> <i> 
                The more important something is, the more prominent it is. For instance, the most important headings are either larger, bolder, in a distinctive color, set off by more white space, or nearer the top of the page—or some combination of the above.
            </i> </h4>
        </div>
        <div class="animation"> <Important/> </div>
       
    </div>

    <div class="point one">
        <div class="animation"> <Noise/> </div>
        <div class="text">
            <h3> 
                Minimize noise
            </h3>
            <h4> Quote: </h4>
            <h4> <i> 
                Users have varying tolerances for complexity and distractions; some people have no problem with busy pages and background noise, but many do. When you’re designing Web pages, it’s probably a good idea to assume that everything is visual noise until proven otherwise.
                </i> </h4>
        </div>
       
       
    </div>

    

    <div class="point one">
        <div class="signup">
            <h2> 
                Sign up to learn more!
            </h2>
            <div class="button" on:click="{() =>correctClick = false}"> <h3>SIGN UP</h3> </div>
            
        </div>
        <div class="smile">
            
        <div class=""   > 
            <Smilyy/>
            <div class="smily" class:hidden={correctClick} >  <Smily/>  </div>
        </div>



    </div>
    </div>


  






<style>

    .button{
        background-color: rgb(146, 193, 227);
        padding: 7px 16px;
        border-radius: 5px;
    }

   .smile{
    position:relative
   }
    .smily{
        position:absolute;
        top:0;

        
    }
   
    .point{
        display: flex;
        gap: 2rem;
        
        width: 100%;
        align-items: center;
    }
    .text{
        width: 50%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 1rem;
        padding-right: 1rem;
    }

    .signup{
        
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 1rem;
        padding-right: 1rem;
    }
    .animation{
        width: 50%;
        
        

    }

   

    .hidden{
        display:none
    }

    .hero{
        padding: 100px 0;
    }

    .one{
        padding: 50px 0;
    }
</style>