<template>
    <header>
        <div class="background"></div>
        <div class="headerText">
            Hello, I'm <span>Juan Carlos Cuadrado</span><br>and I'm a Full Stack developer.
        </div>
        <button @click="scrollToMe('about')">Access</button>
    </header>
</template>

<script>
export default {
    name: "Header",
    methods: {
        scrollToMe(idElement) {
            const element = document.getElementById(idElement);
            element.scrollIntoView({ behavior: "smooth" });
        }
    }
}
</script>

<style scoped>
header {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
span {
    color: #e02a4b;
}
.background {
    position: absolute;
    width: 100%;
    height: 100vh;
    background-image: url("../assets/campito2.jpg");
    background-position: center center;
    background-repeat: no-repeat;
    background-size: 270%;
    filter: blur(10px);
    z-index: -99;
}
.headerText {
    margin: 0px 30px;
    font-size: 45px;
    text-align: center;
    color: black;
}
button {
    margin-top: 30px;
    padding: 10px 35px;
    font-size: 30px;
    background: rgba(0, 0, 0, 0.2);
    color: black;
    border: solid;
    transition: .3s ease;
}
button:hover {
    cursor: pointer;
    background: #1FE0AF;
    color: black;
    border-color: #1FE0AF;
    border-radius: 50px;
}

@media only screen and (max-width: 768px) {
    .background {
        position: absolute;
        width: 100%;
        height: 100vh;
        background-image: url("../assets/campito-mobile.jpg");
        background-position: center center;
        background-size: 150%;
        background-repeat: no-repeat;
        filter: blur(5px);
        z-index: -99;
    }
}
</style>