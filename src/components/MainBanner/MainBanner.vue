<template>
    <div class="main-banner">
        <div class="main-banner-text">
            <h1>Next generation digital banking</h1>
            <h2>
                Take your financial life online.
                Your Easybank account will be a one-stop-shop for spending,
                saving, budgeting, investing, and much more.
            </h2>
            <button type="button">
                Request Invite
            </button>
        </div>
        <div class="main-banner-img">
            <img class="main-banner-img-background desktop" src="../../assets/main-banner/bg-intro-desktop.svg" alt="bg main desktop">
            <img class="main-banner-img-background mobile" src="../../assets/main-banner/bg-intro-mobile.svg" alt="bg main mobile">
            <img class="main-banner-img-front" src="../../assets/main-banner/image-mockups.png" alt="bg front">
        </div>
    </div>

</template>


<style scoped>
    .main-banner {
        display: grid;
        grid-template-columns: 1fr 1fr;
        margin: 0 auto;
        max-width: 1120px;
        height: 656px;
        align-items: center;
    }
    .main-banner-text {
        display: flex;
        align-items: flex-start;
        flex-direction: column;
        justify-content: flex-start;
        margin-right: 25px;
        max-width: 425px;
    }
    .main-banner-text h1 {
        font-size: 3.25rem;
        font-weight: 300;
        line-height: 1.15;
        color: #2d314d;
        margin-bottom: 1.5rem;
    }
    .main-banner-text h2 {
        font-size: 1.125rem;
        font-weight: 300;
        line-height: 1.5;
        color: #9698a6;
        margin-bottom: 2.25rem;
    }
    .main-banner-text button {
        background-image: linear-gradient(to right, #31d35c, #2bb7da);
        padding: 0.875rem 2.1875rem;
        color: #fff;
        font-size: 0.875rem;
        border-radius: 3.125rem;
        border: none;
        text-align: left;
        cursor: pointer;
        transition: opacity 0.2s ease-in;
    }
    .main-banner-text button:hover {
        opacity: 0.8;
    }
    .main-banner-img {
        position: relative;
        align-self: flex-start;
    }
    .main-banner-img .main-banner-img-background {
        position: absolute;
        left: -65px;
        top: -250px;
        z-index: -1;
    }
    .main-banner-img .main-banner-img-background.mobile {
        display: none;
    }
    .main-banner-img .main-banner-img-front {
        position: absolute;
        top: -110px;
        left: 85%;
        transform: translateX(-50%);
        z-index: 1;
    }

    @media(max-width: 767px) {
        .main-banner {
            display: flex;
            flex-direction: column-reverse;
            height: auto;
        }
        .main-banner-text {
            padding: 0 20px;
            margin-right: 0;
            align-items: center;
        }
        .main-banner-text h1 {
            font-size: 36px;
            text-align: center;
        }
        .main-banner-text h2 {
            font-size: 14px;
            text-align: center;
        }
        .main-banner-img .main-banner-img-background {
            position: static;
        }
        .main-banner-img .main-banner-img-front {
            width: 100%;
            left: 50%;
            top: -120px;
        }
        .main-banner-img .main-banner-img-background.desktop {
            display: none;
        }
        .main-banner-img .main-banner-img-background.mobile {
            display: block;
        }

    }
</style>