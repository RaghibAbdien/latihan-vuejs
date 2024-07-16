<template>
    <section>
        <div id="header">
            <h1>Manage your entire community <br> in a single system</h1>
            <span>Who is Nextcent suitable for?</span>
        </div>
        <div id="community">
            <div id="card">
                <div>
                    <img src="../assets/img/membership.png" alt="">
                </div>
                <div>
                    <h1>Membership <br> Organisations</h1>
                    <span>Our membership management <br> software provides full automation of <br> membership renewals and payments</span>
                </div>
            </div>
            <div id="card">
                <div>
                    <img src="../assets/img/buildings.png" alt="">
                </div>
                <div>
                    <h1>National <br> Associations</h1>
                    <span>Our membership management <br> software provides full automation of <br> membership renewals and payments</span>
                </div>
            </div>
            <div id="card">
                <div>
                    <img src="../assets/img/community.png" alt="">
                </div>
                <div>
                    <h1>Clubs And <br> Groups</h1>
                    <span>Our membership management <br> software provides full automation of <br> membership renewals and payments</span>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'CommunitySection'
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
    }

    #header{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        color: #4D4D4D;
        text-align: center;
    }

    h1{
        font-size: 2rem;
        font-weight: 600;
    }

    span{
        font-size: 1rem
    }

    #community{
        margin-top: 3rem;
        display: grid;
        place-items: center;
        grid-template-columns: repeat(3,auto);
        color: #4D4D4D;
        text-align: center;
    }

    #card {
        display: grid;
        gap: 10px;
    }

    #card h1{
        font-size: 1.5rem;
    }

    #card span{
        font-size: .9rem;
    }

    @media (min-width: 320px) and (max-width: 767px){
        h1{
            font-size: 1.5rem;
        }

        #community{
            grid-template-columns: repeat(1,auto);
            gap: 2rem;
        }
    }

    @media (min-width: 768px) and (max-width: 992px){
        #community{
            grid-template-columns: repeat(1,auto);
            gap: 2rem;
        }
    }
</style>