<script>
    import './app.css';
</script>

<header>
    <h1>Oreyly</h1>
</header>

<div class="headerfill"></div>

<main>
    <slot></slot>

</main>



<footer>

    hello :)
</footer>

<style>

    header{
        height: 4rem;
        position: fixed;
        width: 100%;
        background-color: aliceblue;
        padding: 1rem;
    }
    .headerfill{
        height: 4rem;
    }
    main{
        max-width: 900px;
        margin: auto;
        border: 2px solid red;
       
    }


    


</style>