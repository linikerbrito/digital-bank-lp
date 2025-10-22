<template>
    <header :class="{menuOpened: isOpened}">
        <div class="header-container">
            <div>
                <img src="../../assets/geral/logo.svg" alt="Logo">
            </div>
            <div class="header-menu-container">
                <ul class="header-menu">
                    <li>Home</li>
                    <li>About</li>
                    <li>Contact</li>
                    <li>Blog</li>
                    <li>Careers</li>
                </ul>
            </div>
            <div>
                <button type="button" class="header-button" v-if="screenSize === 'desktop'">
                    Request Invite
                </button>
                <button type="button" v-else class="header-button" @click="isOpened = !isOpened">
                    <img src="../../assets/header/icon-hamburger.svg" alt="menu closed icon" class="header-button-closed">
                    <img src="../../assets/header/icon-close.svg" alt="menu opened icon" class="header-button-opened">
                </button>
            </div>
        </div>
    </header>
</template>
<script>
export default {
    data() {
        return {
            isOpened: false
        }
    },
    computed: {
        screenSize() {
            if (window.innerWidth < 768) {
                return 'mobile';
            } else {
                return 'desktop';
            }
        }
    }
}
</script>

<style scoped>
    header {
        background-color: #fff;
        padding: 20px 0;
        width: 100vw;
        display: flex;
        justify-content: center;
        box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
        z-index: 2;
        position: relative;
    }
    .header-container {
        width: 100%;
        max-width: 1120px;
        height: 60px;
        overflow: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .header-menu {
        display: flex;
        align-items: center;
        list-style-type: none;
        margin: 0;
        gap: 20px;
    }
    .header-menu li {
        color: hsl(233, 8%, 62%);
        font-size: 16px;
        font-weight: 500;
        cursor: pointer;
        position: relative;
        height: 60px;
        display: flex;
        align-items: center;
        transition: 0.3s all ease-in;
    }
    .header-menu li:hover {
        color: hsl(233, 26%, 24%);
    }
    .header-menu li::after{
        position: absolute;
        bottom: 0;
        content: "";
        width: 100%;
        height: 5px;
        background: linear-gradient(to right, #31d35c, #2bb7da);
        opacity: 0;
        transition: 0.3s all ease-in;
    }
    .header-menu li:hover::after {
        opacity: 1;
    }
    .header-button {
        padding: 15px 30px;
        border-radius: 20px;
        background: linear-gradient(to right, #31d35c, #2bb7da);
        color: #fff;
        font-weight: 600;
        border: none;
        font-size: 14px;
        cursor: pointer;
        transition: opacity 0.2s ease-in;
    }

    .header-button:hover {
        opacity: 0.8;
    }

    @media (max-width: 1023px) {
        header {
            padding: 20px 0px;
            transition: 0.3s all ease-in;
            position: relative;
        }
        .header-container {
            height: auto;
            width: 100%;
            overflow: hidden;
            padding: 0 10px;
        }
        .header-button {
            background: none;
            padding: 0;
            position: relative;
            width: 24px;
            height: 19px;
        }
        .header-menu-container {
            display: none;
        }
        .menuOpened .header-menu-container {
            position: absolute;
            display: flex;
            top: 84px;
            left: 50%;
            transform: translateX(-50%);
            background-color: #fff;
            z-index: 1;
            border-radius: 5px;
            width: calc(100% - 20px);
        }
        .menuOpened .header-menu {
            width: 100%;
            flex-direction: column;
            align-items: center;
            padding: 25px 0;
            gap: 20px;
        }
        .menuOpened .header-menu li {
            height: auto;
            font-size: 14px;
        }
        .header-button-closed {
            opacity: 1;
            transition: 0.5s all ease-out;
            position: absolute;
            left: 0;
            top: 50%;
            transform: translateY(-50%);
        }
        .menuOpened .header-button-closed {
            opacity: 0;
        }
        .header-button-opened {
            opacity: 0;
            transition: 0.5s all ease-out;
            position: absolute;
            left: 0;
            top: 0;
        }
        .menuOpened .header-button-opened {
            opacity: 1;
        }
        header.menuOpened::after {
            position: fixed;
            top: 64px;
            content: "";
            width: 100%;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.4);
            transition: 0.3s all ease-in;
            z-index: 0;
        }
    }
</style>