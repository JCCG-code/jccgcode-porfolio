<template>
    <nav>
        <div class="menu-burguer">
            <img src="../assets/nav-burguer.png" alt="Menu" @click="viewMenu()">
        </div>

        <transition name="dropdown">
            <div v-if="showMenu == true" class="menu-links">
                <ul>
                    <li><a @click="scrollToMe('topPage')">HOME</a></li>
                    <li><a @click="scrollToMe('about')">ABOUT</a></li>
                    <li><a @click="scrollToMe('portfolio')">PORTFOLIO</a></li>
                    <li><a @click="scrollToMe('blog')">BLOG</a></li>
                    <li><a @click="scrollToMe('contact')">CONTACT</a></li>
                </ul>
            </div>
        </transition>

        <div class="menu-links-desktop">
            <ul>
                <li><a @click="scrollToMe('topPage')">HOME</a></li>
                <li><a @click="scrollToMe('about')">ABOUT</a></li>
                <li><a @click="scrollToMe('portfolio')">PORTFOLIO</a></li>
                <li><a @click="scrollToMe('blog')">BLOG</a></li>
                <li><a @click="scrollToMe('contact')">CONTACT</a></li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
    name: "Menu",
    data() {
        return {
            showMenu: false
        }
    },
    methods: {
        scrollToMe(idElement) {
            // Disable dropdown menu
            this.showMenu = false;

            const element = document.getElementById(idElement);
            element.scrollIntoView({ behavior: "smooth" });
        },
        viewMenu() {
            this.showMenu = !this.showMenu;
        }
    }
}
</script>

<style scoped>
nav {
    position: sticky;
    top: 0;
    z-index: 99;
}
img {
    width: 24px;
}
.menu-burguer {
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: linear-gradient(to right, #1a1919, #3d3d3d);
    opacity: 0.97;
    padding: 20px 0px;
}
.menu-links  {
    position: absolute;
    background-image: linear-gradient(to right, #1a1919, #3d3d3d);
    opacity: 0.97;
    overflow: hidden;
    width: 100%;
}
.menu-links-desktop {
    display: none;
}
li {
    text-align: left;
    color: white;
    font-size: 20px;
    padding-bottom: 20px;
    margin-left: 30px;
}
li:active {
    color: #e02a4b;
}
.dropdown-enter-active, .dropdown-leave-active {
    transition: all .5s ease-in-out;
}
.dropdown-enter-from, .dropdown-leave-to {
    opacity: 0;
}


@media only screen and (min-width: 768px) {
    .menu-burguer, .menu-links {
        display: none;
    }
    .menu-links-desktop {
        position: sticky;
        position: absolute;
        display: flex;
        justify-content: center;
        align-items: center;
        top: 0;
        width: 100%;
        background-image: linear-gradient(to right, #3d3d3d, #1a1919);
        opacity: 0.97;
    }
    li {
        display: inline-block;
        cursor: pointer;
        color: white;
        font-size: 20px;
        margin: 0px 40px;
        padding: 20px 0px;
        transition: .3s ease;
    }
    li:hover {
        color: #e02a4b;
    }
}

</style>