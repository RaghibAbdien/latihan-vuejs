<template>
    <section>
        <div id="#header">
            <h1>Helping a local <br> <span>business reinvent its self</span></h1>
            <span>We reached here with our hard work and dedication</span>
        </div>
        <div id="container">
            <div id="card">
                <img src="../assets/img/user-account.png" alt="">
                <div>
                    <span id="number">2,245,341</span>
                    <p>Members</p>
                </div>
            </div>
            <div id="card">
                <img src="../assets/img/hand.png" alt="">
                <div>
                    <span id="number">46,328</span>
                    <p>Clubs</p>
                </div>
            </div>
            <div id="card">
                <img src="../assets/img/click.png" alt="">
                <div>
                    <span id="number">828,867</span>
                    <p>Event Bookings</p>
                </div>
            </div>
            <div id="card">
                <img src="../assets/img/credit-card.png" alt="">
                <div>
                    <span id="number">1,926,436</span>
                    <p>Payments</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'AchievementSection'
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
        justify-content: space-around;
        align-items: center;
        background: #f5f7fa;
        color: #4D4D4D;
    }

    h1{
        font-size: 2rem;
        font-weight: 600;
    }

    h1 span{
        color: #4CAF4F;
    }

    #container{
        display: grid;
        grid-template-columns: repeat(2,auto);
        row-gap: 4rem;
        column-gap: 4rem;
    }

    #card {
        display: flex;
        align-items: center;
        gap: 1rem;
    }

    #card div {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    #card p {
        font-size: 1em; /* Sesuaikan dengan kebutuhan */
        margin: 2px 0; /* Memberi jarak antara teks */
    }

    #number {
        font-weight: bold;
        font-size: 1.8em; /* Sesuaikan dengan kebutuhan */
    }

    @media (min-width: 320px) and (max-width: 767px){
        section{
            margin: 4rem 3rem;
            flex-direction: column
        }

        #container{
            grid-template-columns: repeat(1,auto);
            margin-top: 2rem;
        }

        #number{
            font-size: 1.2em;
        }
    }

    @media (min-width: 768px) and (max-width: 992px) {
        section{
            margin: 4rem 3rem;
        }

        #container{
            margin-left: 10px;
            row-gap: 1rem;
            column-gap: 1rem;
        }

        #number{
            font-size: 1.5em;
        }
    }

</style>