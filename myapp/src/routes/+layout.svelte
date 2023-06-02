<script>
    import './app.css';
</script>

<header>
    <h1>O´REILLY</h1>

    <div class="button"> <h3>SIGN UP</h3> </div>

   


</header>

<div class="headerfill"></div>

<main>
    <slot></slot>

</main>



<footer>

    
</footer>

<style>

    header{
        height: 4rem;
        position: fixed;
        width: 100%;
        background-color: aliceblue;
        padding: 1rem;
        z-index:2;

        display: flex;
        justify-content: space-between;
        outline: solid 2px  rgb(146, 193, 227);
    }
    .headerfill{
        height: 4rem;
    }
    main{
        max-width: 700px;
        margin: auto;
       
       
    }

    .button{
        background-color: rgb(146, 193, 227);
        padding: 7px 16px;
        border-radius: 5px;
    }


    


</style>