<script>

export default {
    data () {
        return {
            email: null,
            password:null,
            confirmpassword:null,
            error:false
        }
    },
    methods: {
        singupUser()
        {
            console.log(this.email, this.password, this.confirmpassword)

            if (this.password !== this.confirmpassword) {
                this.error = "пароль не совпадает"
            }
            else {
                this.error = ''
            }
        }
    }
}

</script>

<template>
<div class="container">
    <div class="left-container">
        <div>
            <span class="go-back"><b><u>GO BACK</u></b></span>
        </div>
        <div class="icons">
            <img src="https://cdn-icons-png.flaticon.com/128/281/281764.png" width="30px" height="30px" class="icon">
            <img src="https://cdn-icons-png.flaticon.com/128/15/15476.png" height="30px" width="30px" class="icon">
            <img src="https://cdn-icons-png.flaticon.com/128/5968/5968764.png" width="30px" height="30px" class="icon">
            <img src="https://cdn-icons-png.flaticon.com/128/2931/2931618.png" width="30px" height="30px" class="icon">
        </div>

        <div class="dannie">
            <hr class="hr">
            <span><b> Signup via Email </b></span>
            <hr class="hr">
        </div>

        <div class="dannie2">

            <div class="top-dannie">

                <p class="email">Email</p>
                <input type="text" placeholder="@ | Example@gmail.com" class="input" v-model="email">

            </div>

            <div class="top-dannie1">

                    <p class="email">Password</p>
                    <div class="www">
                        <div class="sss">
                            <input type="password" class="input2" v-model="password">
                            <span class="kluch"></span>  
                            <span class="palka">|</span>                     
                        </div>
                        <span class="glaz"></span>
                    </div>

                        <div class="input"></div>

            </div>

            <div class="top-dannie1">

                <p class="email">Confirm Password</p>
                <div class="www">
                        <div class="sss">
                            <input type="password" class="input2" v-model="confirmpassword">
                            <span class="kluch"></span>
                            <span class="palka">|</span>
                        </div>
                        <span class="glaz"></span>
                </div>
                
                <div class="input"></div>

            </div>
            <div class="singup">
                <button class="singuppp" @click="singupUser()">Singup</button>
                <span>{{ this.error }}</span>
                <span class="text">Alredy have an account?, then <u> login </u></span>
            </div>
        </div>

        <div class="end">
            <span>2024 ClickHub</span>
        </div>
    </div>

    <div class="right-container">
            <div class="yellow"></div>
            <div class="yellow-2"></div>
            <div class="yellow-3"></div>
            <div class="yellow-4"></div>
            <div class="white"></div>
            <div class="white-2"></div>
            <div class="white-3"></div>
            <div class="white-4"></div>
            <div class="purple"></div>
            <div class="purple-2"></div>
            <div class="purple-3"></div>
            <div class="purple-4"></div>
            <div class="purple-5"></div>
            <div class="purple-6"></div>
            <div class="green"></div>
            <div class="green-1"></div>
            <div class="green-2"></div>
            <div class="green-3"></div>
            <div class="green-4"></div>
            <div class="green-5"></div>
            <div class="blue"></div>
            <div class="blue-1"></div>
            <div class="blue-2"></div>
            <div class="blue-3"></div>
            <div class="blue-4"></div>
            <div class="red"></div>
            <div class="red-2"></div>
            <div class="red-3"></div>
            <div class="red-4"></div>
    </div>

</div>
</template>

<style scoped>

.purple-2 {
    width: 90px;
    height: 25px;
    border-radius: 20px;
    position: absolute;
    left: 250px;
    transform: rotate(145deg);
    margin-top: 60px;
    background-color: rgb(141, 85, 233);
}

.purple-3 {
    width: 100px;
    height: 20px;
    border-radius: 20px;
    position: absolute;
    left: 20px;
    transform: rotate(145deg);
    margin-top: 180px;
    background-color: #E256E9;
}

.purple-4 {
    width: 200px;
    height: 20px;
    border-radius: 20px;
    position: absolute;
    left: 300px;
    transform: rotate(145deg);
    bottom: 100px;
    background-color: #E256E9;
}

.purple-5 {
    width: 180px;
    height: 10px;
    border-radius: 20px;
    position: absolute;
    left: 300px;
    transform: rotate(145deg);
    bottom: 10px;
    background-color: rgb(141, 85, 233);
}

.purple-6 {
    width: 100px;
    height: 30px;
    border-radius: 20px;
    position: absolute;
    right: 180px;
    transform: rotate(145deg);
    bottom: 270px;
    background-color: #E256E9;
}

.purple {
    width: 200px;
    height: 2px;
    border-radius: 20px;
    position: absolute;
    left: 130px;
    top: -16px;
    transform: rotate(145deg);
    margin-top: 60px;
    background-color: #E256E9;
}

.white {
    width: 200px;
    height: 1px;
    background-color: white;
    position: absolute;
    top: 90px;
    left: 10px;
    transform: rotate(145deg);
}

.white-2 {
    width: 200px;
    height: 1px;
    background-color: white;
    position: absolute;
    top: 360px;
    left: -40px;
    transform: rotate(145deg);
}

.white-3 {
    width: 350px;
    height: 3px;
    background-color: white;
    position: absolute;
    bottom: 180px;
    left: 40px;
    transform: rotate(145deg);
}

.white-4 {
    width: 200px;
    height: 2px;
    background-color: white;
    position: absolute;
    bottom: 100px;
    right: -40px;
    transform: rotate(145deg);
}

.yellow {
    width: 150px;
    height: 20px;
    border-radius: 20px;
    position: absolute;
    left: -40px;
    transform: rotate(150deg);
    margin-top: 60px;
    background-color: #F4DC5A;
}

.yellow-3 {
    width: 150px;
    height: 30px;
    border-radius: 20px;
    position: absolute;
    left: 440px;
    transform: rotate(145deg);
    margin-top: 50px;
    background-color: #F4DC5A;
}

.yellow-2 {
    width: 350px;
    height: 2px;
    border-radius: 20px;
    position: absolute;
    left: 230px;
    transform: rotate(145deg);
    margin-top: 60px;
    background-color: #F4DC5A;
}

.yellow-4 {
    width: 200px;
    height: 1px;
    border-radius: 20px;
    position: absolute;
    right: -30px;
    transform: rotate(145deg);
    bottom: 330px;
    background-color: #F4DC5A;
}


.green {
    width: 300px;
    height: 2px;
    background-color: #214A4A;
    position: absolute;
    top: 230px;
    left: -80px;
    transform: rotate(145deg);
}

.green-1 {
    width: 300px;
    height: 2px;
    background-color: #214A4A;
    position: absolute;
    top: 230px;
    left: 250px;
    transform: rotate(145deg);
}

.green-2 {
    width: 150px;
    height: 25px;
    background-color: #4CC082;
    position: absolute;
    border-radius: 20px;
    bottom: 300px;
    left: 265px;
    transform: rotate(145deg);
}

.green-3 {
    width: 150px;
    height: 15px;
    background-color: #4CC082;
    position: absolute;
    border-radius: 20px;
    bottom: 40px;
    left: -10px;
    transform: rotate(145deg);
}

.green-4 {
    width: 75px;
    height: 35px;
    border-radius: 20px;
    position: absolute;
    left: 250px;
    transform: rotate(145deg);
    bottom: 100px;
    background-color: #4CC082;
}

.green-5 {
    width: 150px;
    height: 15px;
    background-color: #4CC082;
    position: absolute;
    border-radius: 20px;
    bottom: 10px;
    right: -20px;
    transform: rotate(145deg);
}

.blue {
    width: 180px;
    height: 15px;
    border-radius: 20px;
    position: absolute;
    left: 10px;
    transform: rotate(145deg);
    margin-top: 280px;
    background-color: #6E8EFF;
}

.blue-1 {
    width: 100px;
    height: 40px;
    border-radius: 20px;
    position: absolute;
    left: 230px;
    transform: rotate(145deg);
    margin-top: 230px;
    background-color: #6E8EFF;
}

.blue-2 {
    width: 100px;
    height: 25px;
    border-radius: 20px;
    position: absolute;
    left: 50px;
    transform: rotate(145deg);
    bottom: 280px;
    background-color: #6E8EFF;
}

.blue-3 {
    width: 100px;
    height: 25px;
    border-radius: 20px;
    position: absolute;
    right: -23px;
    top: 120px;
    transform: rotate(145deg);
    margin-top: 60px;
    background-color: #6E8EFF;
}

.blue-4 {
    width: 150px;
    height: 15px;
    border-radius: 20px;
    position: absolute;
    right: 10px;
    top: 220px;
    transform: rotate(145deg);
    margin-top: 60px;
    background-color: #6E8EFF;
}

.red {
    width: 250px;
    height: 5px;
    border-radius: 20px;
    position: absolute;
    right: -23px;
    top: 101px;
    transform: rotate(145deg);
    margin-top: 60px;
    background-color: #FF5761;
}

.red-2 {
    width: 300px;
    height: 8px;
    border-radius: 20px;
    position: absolute;
    left: -30px;
    bottom: 250px;
    transform: rotate(145deg);
    margin-top: 60px;
    background-color: #FF5761;
}

.red-3 {
    width: 150px;
    height: 35px;
    border-radius: 20px;
    position: absolute;
    right: -60px;
    bottom: 200px;
    transform: rotate(145deg);
    margin-top: 60px;
    background-color: #FF5761;
}

.red-4 {
    width: 150px;
    height: 10px;
    border-radius: 20px;
    position: absolute;
    right: -60px;
    bottom: 300px;
    transform: rotate(145deg);
    margin-top: 60px;
    background-color: #FF5761;
}

.text {
    font-size: 13px;
}

.sss {
    display: flex;
    justify-content: space-around;
    bottom: -15px;
    position: relative;
    width: 30%;
    left: -45px;
}

.singup {
    display: flex;
    flex-direction: column;
}

.singuppp {
    width: 280px;
    background-color: black;
    margin-top: 30px;
    color: #fff;
    font-size: 20px;
    height: 50px;
    border-radius: 5px;
}

.www {
    display: flex;
    height: 1px;
    justify-content: space-around;
}

.container {
    display: flex;
    font-family: Arial, Helvetica, sans-serif;
}

.left-container {
    width: 900px;
    height: 700px;
    display: flex;
    flex-direction: column;
}

.right-container {
    width: 700px;
    height: 700px;
    background-color: #0A0B2E;
    border-radius: 10px;
    margin-top: 10px;
    position: relative;
    overflow: hidden;
    margin-right: 10px;
}

.header {
    width: 100%;
    height: 70px;
    display: flex;
    justify-content: left;
    align-items: center;
}


.go-back {
    color: black;
    margin-left: 30px;
    font-size: 20px;
}

.welcome {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    margin-top: 20px;
    flex-direction: column;
}

.wel2 {
    font-size: 30px;
}

.wel {
    font-size: 50px
}

.icons {
    margin-top: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.icon {
    background-color: rgb(230, 230, 230);
    margin: 5px;
    padding: 10px;
    border-radius: 10px;
}

.dannie {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 20px;
}

.hr {
    width: 75px;
    margin: 0;
}

.end {
    display: flex;
    height: 200px;
    align-items: flex-end;
    width: 100%;
    justify-content: center;
}


.dannie2 {
    display: flex;
    align-items: center;
    flex-direction: column;
    justify-content: center;
}

.input {
    width: 265px;
    padding-left: 10px;
    height: 40px;
    border-radius: 5px;
    font-size: 15px;
    margin-top: 10px;
    cursor: pointer;
    border: 3px solid;
    background-color: rgb(230, 230, 230);
}

.email {
    margin-bottom: -5px;
}

.kluch {
    background: url(https://cdn-icons-png.flaticon.com/128/2443/2443039.png) no-repeat;
    background-size: 20px;
    width: 20px;
    height: 20px;
    position: relative;
    bottom: -10px;
    left: 20px;
    
}

.glaz {
    background: url(https://cdn-icons-png.flaticon.com/128/158/158746.png) no-repeat;
    background-size: 20px;
    width: 20px;
    position: relative;
    height: 20px;
    bottom: -25px;
}

.palka {
    z-index: 2;
    position: relative;
    color: grey;
    top: 10px;
}

.input2 {
    position: absolute;
    width: 270px;
    height: 40px;
    border-radius: 5px;
    margin-left: 199px;
    border: 3px black solid;
    color: rgb(122, 121, 121);
    margin-top: -5px;
    z-index: 0;
    font-size: 25px;
    text-align: center;
    background-color: rgb(230, 230, 230);
}

</style>