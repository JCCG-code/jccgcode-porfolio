<template>
    <section>
        <h1>CONTACT</h1>
        <p>Have a question or want to work together?</p>

        <form @submit.prevent="handleSubmit" autocomplete="off" ref="form">
            <div class="form">
                <input type="text" name="from_name" placeholder="Name" class="input">
                <input type="email" name="from_email" placeholder="Email" class="input">
                <textarea name="message" placeholder="Your message" class="input textarea"></textarea>
            </div>
            <input type="submit" value="SUBMIT" class="btn-submit">
        </form>

        <div class="arrow-to-top">
            <img src="../assets/arrow.png" alt="LinkedIn" class="icon" @click="scrollToMe('topPage')">
        </div>

        <div class="personal-info">
            <div class="social-networks">
                <div class="icon-background" @click="goTo('https://www.linkedin.com/in/juan-carlos-cuadrado-gracia-166567215/')">
                    <img src="../assets/linkedin-512.png" alt="LinkedIn" class="icon">
                </div>
                <div class="icon-background" @click="goTo('https://www.instagram.com/jccgcode/')">
                    <img src="../assets/instagram-6-512.png" alt="Instagram" class="icon">
                </div>
                <div class="icon-background" @click="goTo('https://www.youtube.com/channel/UCn2VPm-Ys_nhWDwSgdkWm8Q')">
                    <img src="../assets/youtube-512.png" alt="Youtube" class="icon">
                </div>
            </div>
            <p class="name-creator-date">JUAN CARLOS CUADRADO <span>©2022</span></p>
        </div>
            
    </section>
</template>

<script>
import emailjs from '@emailjs/browser'

export default {
    name: "Contact",
    methods: {
        scrollToMe(idElement) {
            // Disable dropdown menu
            this.showMenu = false;

            const element = document.getElementById(idElement);
            element.scrollIntoView({ behavior: "smooth" });
        },
        goTo(url) {
            window.open(url)
        },
        handleSubmit() {
            this.showMessageSuccess = false
            this.showMessageFail = false

            emailjs.sendForm('service_j1xfto7', 'template_altnbe8', this.$refs.form, 'y786t7U4LRgUqoCtT').then((res) => {
                console.log(res)
                this.$refs.form.reset()
            }).catch((err) => {
                console.log(err)
            })
        }
    }
}
</script>

<style scoped>
section {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    width: 100%;
    padding: 70px 0px 0px 0px;
    background-image: linear-gradient(to right, #1a1919, #3d3d3d);
}
h1 {
    margin: 30px 0px;
    font-size: 35px;
    color: rgb(255, 255, 255);
}
p {
    font-weight: bold;
    color: #1FE0AF;
}
form {
    width: 80%;
}
.form {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    margin-top: 40px;
}
.input {
    outline: none;
    width: 100%;
    padding: 12px;
    border: 0px;
    background: rgb(20, 20, 20);
    color: white;
    font-size: 16px;
    margin: 2px 0px;
}
.textarea {
    resize: none;
    height: 190px;
}
.btn-submit {
    display: flex;
    float: right;
    margin-top: 10px;
    padding: 10px 30px;
    font-size: 16px;
    color: white;
    border: 2px solid white;
    background: transparent;
    cursor: pointer;
    transition: .3s ease;
}
.btn-submit:hover {
    border: 2px solid #1FE0AF;
    background: #1FE0AF;
}
.arrow-to-top {
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50px;
    height: 50px;
    background: #e02a4b;
    margin-top: 320px;
    cursor: pointer;
}
.personal-info {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    width: 100%;
    margin-top: 100px;
    padding: 70px 0px;
    background: rgb(30, 30, 30);
}
.social-networks {
    display: flex;
    justify-content: center;
    flex-direction: row;
    align-items: center;
    margin-bottom: 70px;
}
.icon-background {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50px;
    height: 50px;
    margin: 0px 15px;
    background: rgb(50, 50, 50);
    transition: .3s ease;
    cursor: pointer;
}
.icon-background:hover {
    background: #1FE0AF;
}
.icon {
    width: 27px;
}
.name-creator-date {
    font-size: 14px;
    font-weight: normal;
    color: rgb(100, 100, 100);
}
span {
    color: #e02a4b;
    font-weight: 100;
}
.message {
    display: flex;
    justify-content: center;
    align-items: center;
    position: fixed;
    top: 64px;
    background: white;
    border: 2px solid rgb(50, 50, 50);
    width: 100%;
    height: 40px;
}

.infoMessage-enter-active, .infoMessage-leave-active {
    transition-delay: all .5s ease-in-out;
}
.infoMessage-enter-from, .infoMessage-leave-to {
    opacity: 0;
}

@media only screen and (min-width: 1150px) {
    form {
        width: 1000px;
    }
}
</style>