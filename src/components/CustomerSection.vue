<template>
    <section>
        <div>
            <img class="photo" src="../assets/img/customer-section.jpg" alt="">
        </div>
        <div class="customer">
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Aut labore, amet atque animi a rem nesciunt doloribus quasi, esse, sapiente alias! Minima ducimus consequatur eius quasi! Maiores quaerat, accusantium soluta consequuntur hic mollitia, totam inventore a nostrum ducimus at modi unde qui error similique corporis? Inventore similique est soluta praesentium.</p>
            <div class="customer-name">
                <span>Tim Smith</span>
                <span>British Dragon Boat Racing Association</span>
            </div>
            <div class="logo-customer">
                <div class="logo">
                    <img src="../assets/img/facebook.png" alt="">
                    <img src="../assets/img/gitlab.png" alt="">
                    <img src="../assets/img/lightroom.png" alt="">
                    <img src="../assets/img/photoshop.png" alt="">
                    <img src="../assets/img/pinterest.png" alt="">
                    <img src="../assets/img/search.png" alt="">
                </div>
                <div class="link">
                    <a href="">Meet all customers <img src="../assets/img/next.png" alt=""></a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'CustomerSection'
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
        justify-content: space-evenly;
        color: #4D4D4D;
        background: #F5F7FA;
    }

    .photo{
        width: 180px;
        height: 300px;
    }

    .customer{
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }

    p{
        font-size: 1.1em;
        width: 500px;
    }

    .customer-name{
        display: flex;
        flex-direction: column;
        gap: 5px;
    }

    .customer-name span:nth-child(1){
        color: #4CAF4F;
        font-size: 1.2em;
    }

    .customer-name span:nth-child(2){
        color: #a9a9a9;
    }

    .logo-customer{
        margin-top: 10px;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .logo{
        display: flex;
        gap: 20px;
    }
    
    .link a{
        font-size: 1.2em;
        color: #4CAF4F;
    }

    .link img{
        position: relative;
        top: 3px;
    }

    @media (min-width: 320px) and (max-width: 767px){
        section{
            flex-direction: column;
            justify-content: center;
            align-items: center;
            margin: 4rem 0;
        }

        .customer{
            margin-top: 10px;
            justify-content: center;
            align-items: center;
        }

        p{
            width: 300px;
        }

        .logo-customer{
            flex-direction: column;
        }

        .link{
            margin-top: 10px;
        }
    }

    @media (min-width: 768px) and (max-width: 992px){
        section{
            margin: 4rem 3rem;
        }

        .customer{
            margin-left: 10px;
        }
    }
</style>