<template>
    <section>
        <h1>PROJECTS</h1>
        
        <div class="sec-projects">

            <div class="row-projects">
                <!-- Div & Rule Project -->
                <div class="sec-one-project">
                    <img src="../assets/div-and-rule-dapp.png" alt="Div And Rule Screenshot" class="project-img">
                    <div class="sec-project-data">
                        <h2>Div & Rule</h2>
                        <p class="project-description">VueJS / NodeJS</p>
                        <button class="learn-more" @click="showDivAndRule = true">LEARN MORE</button>

                        <!-- Learn more Div And Rule -->
                        <transition name="show-learn-more">
                            <div class="background-learn-more" v-if="showDivAndRule">
                                <div class="learn-more-window">
                                    <button class="close-btn" @click="showDivAndRule = false">x</button>
                                    
                                    <!-- Carrusel -->
                                    <div class="carrusel">
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/div-and-rule-dapp.png" alt="Imagen 1 DAR" class="img-carrusel" v-if="contDAR == 1">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/image1-dar.png" alt="Imagen 1 DAR" class="img-carrusel" v-if="contDAR == 2">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/image2-dar.png" alt="Imagen 2 DAR" class="img-carrusel" v-if="contDAR == 3">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/image3-dar.png" alt="Imagen 3 DAR" class="img-carrusel" v-if="contDAR == 4">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/image4-dar.png" alt="Imagen 4 DAR" class="img-carrusel" v-if="contDAR == 5">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/image5-dar.png" alt="Imagen 5 DAR" class="img-carrusel" v-if="contDAR == 6">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/image6-dar.png" alt="Imagen 6 DAR" class="img-carrusel" v-if="contDAR == 7">
                                        </transition>

                                        <div class="previus-next-btns">
                                            <button class="btn" @click="previusBtn()">&lt;</button>
                                            <button class="btn" @click="nextBtn()">&gt;</button>
                                        </div>
                                        
                                    </div>

                                    <div class="content">
                                        <h3 class="title-content">Div & Rule</h3>
                                        <p class="title-foot">VueJS / NodeJS</p>
                                        <p class="description-content">Div & Rule is a decentralized application developed for my End-Of-Degree project. It is a DApp based on asset tokenization by using the MEVN stack.<br>It is developed through an API RESTful interface and work with BSC network testnet thanks for web3JS communication and smart contracts deployment.</p>
                                        <button class="view-site">VIEW SITE</button>
                                    </div>
                                </div>
                            </div>
                        </transition>
                        
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="sec-one-project">
                    <img src="../assets/default-image.png" alt="Div And Rule Screenshot" class="project-img">
                    <div class="sec-project-data">
                        <h2>Project 2</h2>
                        <p class="project-description">Frontend / Backend</p>
                        <button class="learn-more" @click="showProject2 = true">LEARN MORE</button>

                        <!-- Learn more Div And Rule -->
                        <transition name="show-learn-more">
                            <div class="background-learn-more" v-if="showProject2">
                                <div class="learn-more-window">
                                    <button class="close-btn" @click="showProject2 = false">x</button>
                                    
                                    <!-- Carrusel -->
                                    <div class="carrusel">
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 1 DAR" class="img-carrusel" v-if="contProject2 == 1">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 1 DAR" class="img-carrusel" v-if="contProject2 == 2">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 2 DAR" class="img-carrusel" v-if="contProject2 == 3">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 3 DAR" class="img-carrusel" v-if="contProject2 == 4">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 4 DAR" class="img-carrusel" v-if="contProject2 == 5">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 5 DAR" class="img-carrusel" v-if="contProject2 == 6">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 6 DAR" class="img-carrusel" v-if="contProject2 == 7">
                                        </transition>

                                        <div class="previus-next-btns">
                                            <button class="btn" @click="previusBtn()">&lt;</button>
                                            <button class="btn" @click="nextBtn()">&gt;</button>
                                        </div>
                                        
                                    </div>

                                    <div class="content">
                                        <h3 class="title-content">Project 2</h3>
                                        <p class="title-foot">Frontend / Backend</p>
                                        <p class="description-content">Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default </p>
                                        <button class="view-site">VIEW SITE</button>
                                    </div>
                                </div>
                            </div>
                        </transition>
                        
                    </div>
                </div>                
            </div>

            <div class="row-projects">
                <!-- Project 3 -->
                <div class="sec-one-project">
                    <img src="../assets/default-image.png" alt="Div And Rule Screenshot" class="project-img">
                    <div class="sec-project-data">
                        <h2>Project 3</h2>
                        <p class="project-description">Frontend / Backend</p>
                        <button class="learn-more" @click="showProject3 = true">LEARN MORE</button>

                        <!-- Learn more Div And Rule -->
                        <transition name="show-learn-more">
                            <div class="background-learn-more" v-if="showProject3">
                                <div class="learn-more-window">
                                    <button class="close-btn" @click="showProject3 = false">x</button>
                                    
                                    <!-- Carrusel -->
                                    <div class="carrusel">
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 1 DAR" class="img-carrusel" v-if="contProject3 == 1">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 1 DAR" class="img-carrusel" v-if="contProject3 == 2">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 2 DAR" class="img-carrusel" v-if="contProject3 == 3">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 3 DAR" class="img-carrusel" v-if="contProject3 == 4">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 4 DAR" class="img-carrusel" v-if="contProject3 == 5">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 5 DAR" class="img-carrusel" v-if="contProject3 == 6">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 6 DAR" class="img-carrusel" v-if="contProject3 == 7">
                                        </transition>

                                        <div class="previus-next-btns">
                                            <button class="btn" @click="previusBtn()">&lt;</button>
                                            <button class="btn" @click="nextBtn()">&gt;</button>
                                        </div>
                                        
                                    </div>

                                    <div class="content">
                                        <h3 class="title-content">Project 3</h3>
                                        <p class="title-foot">Frontend / Backend</p>
                                        <p class="description-content">Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default </p>
                                        <button class="view-site">VIEW SITE</button>
                                    </div>
                                </div>
                            </div>
                        </transition>
                        
                    </div>
                </div>

                <!-- Project 4 -->
                <div class="sec-one-project">
                    <img src="../assets/default-image.png" alt="Div And Rule Screenshot" class="project-img">
                    <div class="sec-project-data">
                        <h2>Project 4</h2>
                        <p class="project-description">Frontend / Backend</p>
                        <button class="learn-more" @click="showProject4 = true">LEARN MORE</button>

                        <!-- Learn more Div And Rule -->
                        <transition name="show-learn-more">
                            <div class="background-learn-more" v-if="showProject4">
                                <div class="learn-more-window">
                                    <button class="close-btn" @click="showProject4 = false">x</button>
                                    
                                    <!-- Carrusel -->
                                    <div class="carrusel">
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 1 DAR" class="img-carrusel" v-if="contProject4 == 1">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 1 DAR" class="img-carrusel" v-if="contProject4 == 2">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 2 DAR" class="img-carrusel" v-if="contProject4 == 3">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 3 DAR" class="img-carrusel" v-if="contProject4 == 4">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 4 DAR" class="img-carrusel" v-if="contProject4 == 5">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 5 DAR" class="img-carrusel" v-if="contProject4 == 6">
                                        </transition>
                                        <transition name="carrusel-trans" mode="out-in">
                                            <img src="../assets/default-image.png" alt="Imagen 6 DAR" class="img-carrusel" v-if="contProject4 == 7">
                                        </transition>

                                        <div class="previus-next-btns">
                                            <button class="btn" @click="previusBtn()">&lt;</button>
                                            <button class="btn" @click="nextBtn()">&gt;</button>
                                        </div>
                                        
                                    </div>

                                    <div class="content">
                                        <h3 class="title-content">Project 4</h3>
                                        <p class="title-foot">Frontend / Backend</p>
                                        <p class="description-content">Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default Default </p>
                                        <button class="view-site">VIEW SITE</button>
                                    </div>
                                </div>
                            </div>
                        </transition>
                        
                    </div>
                </div>                
            </div>

        </div>
    </section>
</template>

<script>
export default {
    name: "Portfolio",
    data() {
        return {
            showDivAndRule: false,
            showProject2: false,
            showProject3: false,
            showProject4: false,
            contDAR: 1,
            contProject2: 1,
            contProject3: 1,
            contProject4: 1
        }
    },
    methods: {
        previusBtn() {
            if (this.contDAR > 1) {
                this.contDAR--
            } else {
                this.contDAR = 7
            }
        },
        nextBtn() {
            if (this.contDAR < 7) {
                this.contDAR++
            } else {
                this.contDAR = 1
            }
        }
    }
}
</script>

<style scoped>
section {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    padding: 70px 0px 120px 0px;
    background-color: rgb(240, 240, 240);
}
h1 {
    margin: 30px 0px;
    font-size: 35px;
    color: rgb(50, 50, 50);
}
h2 {
    position: relative;
    margin: 10px 0px;
    font-size: 20px;
    color: rgb(50, 50, 50);
}
.sec-projects {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    margin: 50px 0px;
}
.sec-one-project {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}
.project-img {
    width: 100%;
    filter: blur(5px);
}
.sec-project-data {
    position: absolute;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}
.project-description {
    position: relative;
    color: #e02a4b;
    font-size: 12px;
    margin-top: -12px;
    margin-bottom: 20px;
}
.learn-more {
    position: relative;
    padding: 5px 25px;
    font-size: 15px;
    color: black;
    border: solid #e02a4b;
    margin: 20px 0px;
    transition: .3s ease;
}
.learn-more:hover {
    cursor: pointer;
    background: #e02a4b;
    color: white;
}
.background-learn-more {
    position: fixed;
    display: flex;
    justify-content: center;
    top: 0;
    width: 100%;
    height: 100vh;
    background: rgba(0, 0, 0, 0.3);
    z-index: 99;
}
.learn-more-window {
    position: relative;
    top: 64px;
    width: 100%;
    height: min-content;
    padding-bottom: 15px;
    background: white;
    box-shadow: 0px 1px 10px rgb(50, 50, 50);
}
.close-btn {
    position: absolute;
    right: 0;
    margin: 20px 20px;
    padding: 0px 15px;
    padding-bottom: 5px;
    font-size: 30px;
    color: rgb(50, 50, 50);
    border: 0px;
    border-radius: 10px;
    background: rgb(240, 240, 240);
    cursor: pointer;
}
.img-carrusel {
    width: 100%;
}
.previus-next-btns {
    display: flex;
    justify-content: space-between;
}
.btn {
    margin-top: -5px;
    padding: 10px 50px;
    padding-bottom: 5px;
    font-size: 20px;
    color: rgb(50, 50, 50);
    border: 0px;
    background: rgb(240, 240, 240);
    cursor: pointer;
}
.title-content {
    font-size: 30px;
    margin: 35px 30px;
    color: rgb(50, 50, 50);
}
.title-foot {
    font-size: 20px;
    margin: -10px 0px 20px 30px;
    color: rgb(120, 120, 120);
}
.description-content {
    font-size: 14px;
    margin: 30px 30px;
    color: rgb(50, 50, 50);
}
.view-site {
    padding: 7px 27px;
    margin: 0px 30px;
    font-size: 15px;
    color: white;
    border: 0px;
    background: #e02a4b;
    transition: .3s ease;
}
.view-site:hover {
    cursor: pointer;
    background: white;
    color: #e02a4b;
}
.show-learn-more-enter-active, .show-learn-more-leave-active {
    transition: all .5s ease-in-out;
}
.show-learn-more-enter-from, .show-learn-more-leave-to {
    opacity: 0;
}
.carrusel-trans-enter-active, .carrusel-trans-leave-active {
    transition: all .5s ease-in-out;
    position: relative;
}
.carrusel-trans-enter-from, .carrusel-trans-leave-to {
    position: absolute;
    opacity: 0;
}

@media only screen and (min-width: 768px) {
    .row-projects {
        display: flex;
        justify-content: center;
        flex-direction: row;
        align-items: center;
    }
    .sec-one-project {
        width: 50%;
    }
    .background-learn-more {
        left: 0;
    }
    .learn-more-window {
        position: relative;
        width: 50%;
        background: white;
        box-shadow: 0px 1px 10px rgb(50, 50, 50);
    }
}

@media only screen and (min-width: 1150px) {
    .sec-one-project {
        width: 70vh;
    }
}
</style>