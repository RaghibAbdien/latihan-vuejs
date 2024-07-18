<template>
    <div>
        <div class="footer-head">
            <h1>Pellentesque suscipit <br> fringilla ilbero eu.</h1>
            <button>Get a Demo <img class="arrow" src="../assets/img/next-putih.png" alt=""></button>
        </div>
        <div class="footer-body">
            <div class="company-info">
                <div class="brand">
                    <img src="../assets/img/bird.png" alt="">
                    <span class="logo">Nextcent</span>
                </div>
                <div class="copyright">
                    <span>Copyright © 2024 Nexcent ltd.</span>
                    <span>All right reserved</span>
                </div>
                <div class="icon">
                    <div>
                        <img src="../assets/img/instagram-logo.png" alt="">
                    </div>
                    <div>
                        <img src="../assets/img/basketball.png" alt="">
                    </div>
                    <div>
                        <img src="../assets/img/twitter-logo.png" alt="">
                    </div>
                    <div>
                        <img src="../assets/img/youtube-putih.png" alt="">
                    </div>
                </div>
            </div>
            <div class="links">
                <div>
                    <span>Company</span>
                    <ul>
                        <li><a href="">About us</a></li>
                        <li><a href="">Blog</a></li>
                        <li><a href="">Contact us</a></li>
                        <li><a href="">Pricing</a></li>
                        <li><a href="">Testimonials</a></li>
                    </ul>
                </div>
                <div>
                    <span>Support</span>
                    <ul>
                        <li><a href="">Help center</a></li>
                        <li><a href="">Terms of service</a></li>
                        <li><a href="">Legal</a></li>
                        <li><a href="">Privacy policy</a></li>
                        <li><a href="">Status</a></li>
                    </ul>
                </div>
                <div>
                    <span>Stay up to date</span>
                    <div class="send">
                        <input placeholder="Your Email Address" type="text">
                        <img src="../assets/img/send.png" alt="">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterSection'
    }
</script>

<style scoped>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: sans-serif;
    }

    .footer-head{
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        color: #4D4D4D;
        margin-bottom: 2rem;
    }

    h1{
        font-weight: 600;
        font-size: 3em;
        text-align: center;
    }

    button{
        margin-top: 20px;
        background: #4CAF4F;
        padding: .8rem 2rem;
        border-radius: 5px;
        color: #fff;
        font-size: 1.1em;
        font-weight: 600;
    }

    .arrow{
        position: relative;
        top: 3px;
        left: 3px;
    }

    .footer-body{
        background: #263238;
        color: #fff;
        padding: 2.5rem 8rem;
        display: flex;
        gap: 15rem;
    }

    .company-info{
        display: flex;
        flex-direction: column;
        gap: 2rem;
    }

    .brand{
        display: flex;
        align-items: center;
        justify-content: start;
        gap: 5px;
    }

    span.logo{
        font-size: 30px;
        font-family: monospace;
        font-weight: 600;
    }

    .copyright{
        display: flex;
        flex-direction: column;
    }

    .icon{
        display: flex;
        gap: 10px;
    }

    .icon div{
        padding: 8px 10px;
        background: #545454;
        border-radius: 999px;
        display: grid;
        place-items: center;
    }

    .links{
        display: flex;
        width: 100%;
        justify-content: space-between
    }

    .links span{
        font-size: 1.2em;
        font-weight: 500;
    }

    .links ul{
        margin-top: 20px;
        display: flex;
        flex-direction: column;
        gap: 10px;
    }

    .links a{
        color: #fff;
    }

    .send{
        background: #545454;
        padding: 10px;
        border-radius: 5px;
        display: flex;
        margin-top: 20px;
    }

    input{
        outline: none;
        background: none;
        border: none;
        color: #fff;
        width: 150px;
    }

    input::placeholder{
        color: #fff;
    }

    @media (min-width: 320px) and (max-width: 767px) {
        .footer-body{
            padding: 1.5rem 1rem;
            gap: 4rem;
            flex-direction: column;
            align-items: center;
        }

        input{
            width: 30vw;
            max-width: 150px;
            box-sizing: border-box;
        }
    }

    @media (min-width: 768px) and (max-width: 992px) {
        .footer-body{
            gap: 5rem;
            padding: 2rem 4rem;
        }
    }

</style>