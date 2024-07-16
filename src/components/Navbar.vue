<template>
    <nav>
        <div class="brand">
            <img src="../assets/img/bird.png" alt="logo">
            <span class="logo">Nextcen</span>
        </div>
        <div>
            <ul :class="{ open: isMenuOpen}">
                <li><a class="active" href="">Home</a></li>
                <li><a href="">Service</a></li>
                <li><a href="">Feature</a></li>
                <li><a href="">Product</a></li>
                <li><a href="">Testimonial</a></li>
                <li><a href="">FAQ</a></li>
            </ul>
        </div>
        <div class="btn">
            <button>Login</button>
            <button>Sign Up</button>
        </div>
        <div id="menu-bar">
            <input id="check" type="checkbox" v-model="isMenuOpen">
            <label for="check">
                <img src="../assets/img/more.png">
            </label>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'Navbar',
    data(){
        return {
            isMenuOpen: false
        }
    }
}
</script>

<style lang="css" scoped>

nav{
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 5px 20px;
}

div.brand{
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 5px;
}

span.logo{
    font-size: 30px;
    font-family: monospace;
    font-weight: 600;
    color: #717171;
}

nav ul li{
    display: inline-block;
    margin: 0 8px;
}

nav ul li a{
    color: #606060;
    font-weight: 500;
}

a.active, a:hover{
    color: #2b2b2b;
    padding: 2px 0;
    border-bottom: 1px solid black;
}

.btn{
    display: flex;
    gap: 5px;
}

.btn button{
    font-size: 1rem;
    color: #f5f7fa;
    background: #43a046;
    padding: 7px 15px;
    border-radius: 3px;
}

.btn button:hover{
    background: #388e3b;
}

.btn button:first-child{
    background: #f5f7fa;
    color: #43a046;
}

.btn button:first-child:hover{
    background: #ccd0d3;
}

#menu-bar{
    display: none;
}

#check{
    display: none;
}

@media (max-width: 320px){

    span.logo{
        font-size: 20px
    }

    .btn button{
        font-size: small;
    }
}

@media (max-width: 768px){
    
    nav ul{
        padding: 15px 0;
        position: fixed;
        width: 100%;
        height: 100vh;
        background: #89939e;
        top: -100vh;
        left: 0;
        text-align: center;
        transition: all 0.5s;
    }

    nav ul.open{
        top: 50px;
    }

    nav ul li{
        display: block;
        margin-bottom: 1rem;
    }

    .btn{
        margin-right: 10px;
    }

    #menu-bar{
        display: block;
    }

    #menu-bar label img{
        cursor: pointer;
    }
}
</style>