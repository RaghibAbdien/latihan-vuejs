<template>
    <section>
        <img src="../assets/img/unlock-section.svg" alt="">
        <div>
            <h1>The unseen of spending three <br> years at Pixelgrade</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eos quasi totam eius neque quia vero dolor? Architecto iste corporis tempore odio. Tempora velit facere, iusto nam explicabo sed autem fugit. Excepturi ad vel adipisci numquam ipsa possimus, similique culpa mollitia voluptatem doloremque, id repellendus perspiciatis consectetur eveniet voluptates, magni assumenda.</p>
            <button>Learn More</button>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'UnlockSection'
    }
</script>

<style scoped>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: sans-serif;
    }

    section{
        margin: 4rem 10rem;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    img{
        width: 450px;
        height: 450px;
    }

    div{
        display: flex;
        flex-direction: column;
        align-items: start;
        justify-content: center;
        color: #4D4D4D;
        gap: 1.5rem;
    }

    h1{
        font-size: 2rem;
        font-weight: 600;
    }

    p{
        text-align: justify;
    }

    button{
        padding: 1rem 2rem;
        background: #4CAF4F;
        border-radius: 3px;
        font-size: 1rem;
        color: #fff;
    }

    button:hover{
        background: #58c35c;
    }

    @media (min-width: 320px) and (max-width: 767px){
        section{
            margin: 4rem 4rem;
            flex-direction: column;
        }

        img{
            width: 200px;
            height: 200px;
        }

        h1{
            font-size: 1.5rem;
        }
    }

    @media (min-width: 768px) and (max-width: 992px){
        section{
            margin: 4rem;
        }

        img{
            width: 250px;
            height: 250px;
        }
    }
</style>