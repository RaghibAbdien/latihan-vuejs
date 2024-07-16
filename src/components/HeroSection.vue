<template>
    <section>
        <div>
            <h1>Lessons and insights <br> <p>from 8 years</p></h1>
            <span>Where to grow your business as a photographer: site or social media?</span>
            <div>
                <button id="register">Register</button>
            </div>
        </div>
        <div>
            <img src="../assets/img/hero-section.svg" alt="">
        </div>
    </section>
</template>

<script>
    export default {
        name: 'HeroSection',
    }
</script>

<style lang="css" scoped>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-family: sans-serif;
    }


    section{
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin: 3rem 5rem;
    }

    section div:first-child{
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    section div:first-child h1{
        font-size: 4rem;
        color: #4D4D4D;
    }

    section div:first-child h1 p{
        color: #4CAF4F;
    }

    section div:first-child span{
        color: #717171;
    }

    section div:first-child button{
        padding: 0;
    }

    #register{
        margin: 15px 0;
        padding: 1rem 2rem;
        border-radius: 3px;
        background: #4CAF4F;
        font-size: 1rem;
    }

    #register:hover{
        background: #58c35c;
    }

    img{
        width: 400px;
        height: 400px;
    }

    @media (min-width: 320px){
        section{
            margin: 1rem 2rem;
        }

        section div:first-child h1{
            font-size: 1.2rem
        }

        section div:first-child span{
            font-size: .8rem;
        }   

        img{
            width: 120px;
            height: 120px;
        }

        #register{
            padding: .8rem 1.5rem;
        }
    }

    @media (min-width: 768px){

        section{
            margin: .8rem 3rem;
        }

        section div:first-child h1{
            font-size: 2rem
        }

        section div:first-child span{
            font-size: 1rem;
        }

        img{
            width: 300px;
            height: 300px;
        }
    }

    @media (min-width: 992px){

        section{
            margin: 1rem 5rem;
        }

        section div:first-child h1{
            font-size: 4rem
        }

        section div:first-child span{
            font-size: 1.2rem;
        }

        img{
            width: 400px;
            height: 400px;
        }
    }

</style>