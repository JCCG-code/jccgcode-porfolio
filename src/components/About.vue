<template>
    <section>
        <h1>ABOUT</h1>

        <!-- Logo section describing myself -->
        <div class="sec-logos">
            <div class="row-logos">
                <div class="indiv-logo">
                    <img class="logo" src="../assets/rocket.png" alt="Rocket logo">
                    <h2>Dynamic</h2>
                    <p>Trying to develop web pages which seem to be alive</p>
                </div>
                <div class="indiv-logo">
                    <img class="logo" src="../assets/search.png" alt="Search logo">
                    <h2>Curious</h2>
                    <p>Finding out and researching how to work with new technologies</p>
                </div>
            </div>
            <div class="row-logos">
                <div class="indiv-logo">
                    <img class="logo" src="../assets/time.png" alt="Time logo">
                    <h2>Fast</h2>
                    <p>Trying to give the best of myself in the fastest and most secure way</p>
                </div>
                <div class="indiv-logo">
                    <img class="logo" src="../assets/solutions.png" alt="Solutions logo">
                    <h2>Intuitive</h2>
                    <p>Programming in the easiest way without reinventing the wheel</p>
                </div>
            </div>
        </div>

        <div class="second-section">
            <!-- Photo and short description-->
            <div class="sec-photo-description">
                <img class="photo" src="../assets/photoJCCG2.jpg" alt="Photo JCCG">
                <h2>Who am I?</h2>
                <p class="description-myself">
                    I am a Full Stack developer interest in new and innovative technologies. I always try to develop web pages with dynamic, intuitive and responsive user experience.
                </p>
            </div>

            <!-- Skills -->
            <div class="sec-my-skills">

                <h2 class="skills-title" @click="showFrontend = !showFrontend">Front-End skills</h2>

                <transition name="wrap-trans">
                    <div v-if="showFrontend" class="wrap-languages">
                        <div class="language-percent">
                            <div class="language-name">Vue</div>
                            <div class="percent-background">
                                <div class="percent-vue"></div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name">HTML</div>
                            <div class="percent-background">
                                <div class="percent-html"></div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name">CSS</div>
                            <div class="percent-background">
                                <div class="percent-css"></div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name">Javascript</div>
                            <div class="percent-background">
                                <div class="percent-javascript"></div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name">Web3.js</div>
                            <div class="percent-background">
                                <div class="percent-web3js"></div>
                            </div>
                        </div>
                    </div>
                </transition>

                <h2 class="skills-title" @click="showBackend = !showBackend">Back-End skills</h2>
                
                <transition name="wrap-trans">
                    <div v-if="showBackend" class="wrap-languages">
                        <div class="language-percent">
                            <div class="language-name">Node.js</div>
                            <div class="percent-background">
                                <div class="percent-nodejs"></div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name">Express.js</div>
                            <div class="percent-background">
                                <div class="percent-expressjs"></div>
                            </div>
                        </div>
                    </div>
                </transition>

                <h2 class="skills-title" @click="showDatabase = !showDatabase">Database skills</h2>

                <transition name="wrap-trans">
                    <div v-if="showDatabase" class="wrap-languages">
                        <div class="language-percent">
                            <div class="language-name">MySQL</div>
                            <div class="percent-background">
                                <div class="percent-mysql"></div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name">MongoDB</div>
                            <div class="percent-background">
                                <div class="percent-mongodb"></div>
                            </div>
                        </div>
                    </div>
                </transition>
                
                <h2 class="skills-title" @click="showTechnologies = !showTechnologies">Technologies</h2>

                <transition name="wrap-trans">
                    <div v-if="showTechnologies" class="wrap-languages">
                        <div class="language-percent">
                            <div class="language-name">API RESTful</div>
                            <div class="percent-background">
                                <div class="percent-apirestful"></div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name">Blockchain</div>
                            <div class="percent-background">
                                <div class="percent-blockchain"></div>
                            </div>
                        </div>
                    </div>
                </transition>

                <h2 class="skills-title" @click="showOtherLanguages = !showOtherLanguages">Other languages</h2>

                <transition name="wrap-trans">
                    <div v-if="showOtherLanguages" class="wrap-languages">
                        <div class="language-percent">
                            <div class="language-name">C/C++</div>
                            <div class="percent-background">
                                <div class="percent-c"></div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name">Bash</div>
                            <div class="percent-background">
                                <div class="percent-bash"></div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name">Solidity</div>
                            <div class="percent-background">
                                <div class="percent-solidity"></div>
                            </div>
                        </div>
                    </div>
                </transition>

                <h2 class="skills-title" @click="showLearning = !showLearning">Learning</h2>

                <transition name="wrap-trans">
                    <div v-if="showLearning" class="wrap-languages">
                        <div class="language-percent">
                            <div class="language-name-learning">PHP</div>
                            <div class="percent-background">
                                <div class="percent-inprocess">In process...</div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name-learning">Angular</div>
                            <div class="percent-background">
                                <div class="percent-inprocess">In process...</div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name-learning">React</div>
                            <div class="percent-background">
                                <div class="percent-inprocess">In process...</div>
                            </div>
                        </div>
                        <div class="language-percent">
                            <div class="language-name-learning">Python</div>
                            <div class="percent-background">
                                <div class="percent-inprocess">In process...</div>
                            </div>
                        </div>
                    </div>
                </transition>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "About",
    data() {
        return {
            showFrontend: false,
            showBackend: false,
            showDatabase: false,
            showTechnologies: false,
            showOtherLanguages: false,
            showLearning: false
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
}
h1 {
    margin: 30px 0px;
    font-size: 35px;
    color: rgb(50, 50, 50);
}
h2 {
    margin: 10px 0px;
    font-size: 20px;
    color: rgb(50, 50, 50);
}
.sec-logos {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    width: 100%;
}
.row-logos {
    display: flex;
    justify-content: space-around;
    flex-direction: row;
    align-items: center;
    width: 90%;
}
.indiv-logo {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    margin: 10px 0px;
}
.logo {
    width: 90px;
}
p {
    text-align: center;
    color: rgb(50, 50, 50);
    font-size: 12px;
    margin: 10px 0px;
    width: 150px;
}
.second-section {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}
.sec-photo-description {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    margin: 20px 0px;
}
.photo {
    width: 215px;
    margin: 18px 0px;
}
.description-myself {
    text-align: center;
    color: rgb(50, 50, 50);
    font-size: 14px;
    width: 80%;
}
.sec-my-skills {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    width: 90%;
}
.skills-title {
    text-align: center;
    color: white;
    font-size: 18px;
    background: linear-gradient(to right, #1a1919, #626262);
    width: 90%;
    padding: 10px 0px;
    cursor: pointer;
}
.wrap-trans-enter-active, .wrap-trans-leave-active {
    transition: all .5s ease-in-out;
}
.wrap-trans-enter-from, .wrap-trans-leave-to {
    transform: translateX(30px);
    opacity: 0;
}
.wrap-languages {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    width: 90%;
}
.language-percent {
    display: flex;
    justify-content: center;
    flex-direction: row;
    align-items: center;
    width: 100%;
    margin-bottom: 7px;
}
.language-name {
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
    font-size: 12px;
    font-weight: bold;
    background: #1FE0AF;
    width: 90px;
    height: 25px;
}
.language-name-learning {
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
    font-size: 12px;
    font-weight: bold;
    background: #1face0;
    width: 90px;
    height: 25px;
}
.percent-background {
    width: 91%;
    height: 25px;
    background-color: #dfdfdf;
}
.percent-html, .percent-css, .percent-javascript {
    position: relative;
    background: #189475;
    width: 90%;
    height: 25px;
}
.percent-vue, .percent-nodejs, .percent-expressjs {
    position: relative;
    background: #189475;
    width: 80%;
    height: 25px;
}
.percent-mysql, .percent-mongodb {
    position: relative;
    background: #189475;
    width: 70%;
    height: 25px;
}
.percent-web3js, .percent-apirestful, .percent-blockchain, .percent-c, .percent-cpp {
    position: relative;
    background: #189475;
    width: 60%;
    height: 25px;
}
.percent-bash, .percent-solidity {
    position: relative;
    background: #189475;
    width: 50%;
    height: 25px;
}
.percent-inprocess {
    position: relative;
    display: flex;
    text-align: center;
    justify-content: center;
    align-items: center;
    color: white;
    font-size: 14px;
    background: #1e7290;
    width: 35%;
    height: 25px;
}

@media only screen and (min-width: 768px) {
    .logo {
        width: 130px;
    }
    h2 {
        font-size: 25px;
    }
    p {
        text-align: center;
        color: rgb(50, 50, 50);
        font-size: 16px;
        margin: 10px 0px;
        width: 280px;
    }
    .photo {
        width: 260px;
        margin: 18px 0px;
    }
    .description-myself {
        text-align: center;
        color: rgb(50, 50, 50);
        font-size: 16px;
        width: 80%;
    }
}

@media only screen and (min-width: 1150px) {
    p {
        text-align: center;
        color: rgb(50, 50, 50);
        font-size: 18px;
        margin: 10px 0px;
        width: 280px;
    }
    .description-myself {
        text-align: center;
        color: rgb(50, 50, 50);
        font-size: 18px;
        width: 80%;
    }
    .sec-logos {
        display: flex;
        justify-content: center;
        flex-direction: row;
        align-items: center;
        width: 100%;
        margin: 50px 0px;
    }
    .sec-photo-description {
        margin: 0;
    }
    .second-section {
        display: flex;
        justify-content: center;
        flex-direction: row;
        align-items: center;
    }
    .photo {
        width: 300px;
        margin: 50px 0px;
    }
}
</style>