<template>
    <section>
        <div>
            <h1>Caring is the new marketing</h1>
            <p>The Nexcent blog is the best place to read about the latest membership insights, trends and more. See who's joining the community, read about how our community are increasing their membership income and lot's more.​</p>
        </div>
        <div class="container">
            <div class="card">
                <img class="bg" src="../assets/img/caring1.jpg" alt="">
                <div class="card-body">
                    <h4>Creating Streamlined Safeguarding Processes with OneRen</h4>
                    <a href="">Readmore <img class="arrow" src="../assets/img/next.png" alt=""></a>
                </div>
            </div>
            <div class="card">
                <img class="bg" src="../assets/img/caring2.jpg" alt="">
                <div class="card-body">
                    <h4>What are your safeguarding responsibilities and how can you manage them?</h4>
                    <a href="">Readmore <img class="arrow" src="../assets/img/next.png" alt=""></a>
                </div>
            </div>
            <div class="card">
                <img class="bg" src="../assets/img/caring3.jpg" alt="">
                <div class="card-body">
                    <h4>Revamping the Membership Model with Triathlon Australia</h4>
                    <a href="">Readmore <img class="arrow" src="../assets/img/next.png" alt=""></a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'CommunityUpdateSection'
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
        margin: 4rem 5rem;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        color: #4D4D4D;
    }

    h1{
        text-align: center;
        font-size: 2em;
        font-weight: 600;
    }

    p{
        width: 500px;
        text-align: center;
    }

    .container{
        margin-top: 2rem;
        display: grid;
        grid-template-columns: repeat(3,auto);
        column-gap: 20px;
    }

    .card{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }

    .bg{
        width: 350px;
        height: 200px;
        border-radius: 10px;
    }

    .card-body{
        position: relative;
        bottom: 100px;
        width: 250px;
        background: #F5F7FA;
        border-radius: 10px;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1rem;
        padding: 10px;
        box-shadow: 2px 12px 5px -2px rgba(179,179,179,0.5);
        -webkit-box-shadow: 2px 12px 5px -2px rgba(179,179,179,0.5);
        -moz-box-shadow: 2px 12px 5px -2px rgba(179,179,179,0.5);
    }

    .card-body h4{
        font-weight: 700;
        font-size: 1.1em;
        text-align: center;
    }

    .card-body a{
        color: #4CAF4F;
    }

    .arrow{
        position: relative;
        top: 3px;
        left: 3px;
    }

    @media (min-width: 320px) and (max-width: 767px){
        section{
            margin: 4rem 2rem;
        }

        p{
            width: 300px;
        }

        .container{
            grid-template-columns: repeat(1,auto);
        }
    }

    @media (min-width: 768px) and (max-width: 992px) {
        .container{
            grid-template-columns: repeat(2,auto);
        }

        .container .card:nth-child(3) {
            grid-column: 1 / span 2;
            justify-self: center;
        }
    }
</style>