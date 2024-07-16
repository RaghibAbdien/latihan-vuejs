<template>
    <section>
        <div>
            <h1>Our Client</h1>
            <span>We have been working with some Fortune 500+ clients</span>
        </div>
        <div id="clients">
            <img src="../assets/img/facebook.png" alt="">
            <img src="../assets/img/gitlab.png" alt="">
            <img src="../assets/img/lightroom.png" alt="">
            <img src="../assets/img/photoshop.png" alt="">
            <img src="../assets/img/pinterest.png" alt="">
            <img src="../assets/img/search.png" alt="">
            <img src="../assets/img/youtube.png" alt="">
        </div>
    </section>
</template>

<script>
    export default {
        name: 'ClientSection'
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
        margin: 3rem 5rem;
    }

    section div:first-child{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        color: #4D4D4D;
    }

    h1{
        font-size: 2rem;
        font-weight: 600;
    }

    span{
        text-align: center;
        font-size: 1rem;
    }

    #clients{
        margin-top: 3rem;
        display: grid;
        place-items: center;
        grid-template-columns: repeat(7,auto);
    }
</style>