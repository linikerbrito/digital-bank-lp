<template>
    <section class="benefits-container">
        <div>
            <div class="benefits-top">
                <h2>Why choose Easybank?</h2>
                <h3>
                    We leverage Open Banking to turn your bank account into your financial hub. Control your finances like never before.
                </h3>
            </div>
            <div class="benefits-cards">
                <div class="benefits-card">
                    <img src="../../assets/benefits/icon-online.svg" width="72" height="72" alt="">
                    <span>Online Banking</span>
                    <p>
                        Our modern web and mobile applications allow you to keep track of your finances wherever you are in the world.
                    </p>
                </div>
                <div class="benefits-card">
                    <img src="../../assets/benefits/icon-online.svg" width="72" height="72" alt="">
                    <span>Simple Budgeting</span>
                    <p>
						See exactly where your money goes each month. Receive notifications when you’re close to hitting your limits.
                    </p>
                </div>
                <div class="benefits-card">
                    <img src="../../assets/benefits/icon-online.svg" width="72" height="72" alt="">
                    <span>Fast Onboarding</span>
                    <p>
                        We don’t do branches. Open your account in minutes online and start taking control of your finances right away.
                    </p>
                </div>
                <div class="benefits-card">
                    <img src="../../assets/benefits/icon-online.svg" width="72" height="72" alt="">
                    <span>Open API</span>
                    <p>
                        Manage your savings, investments, pension, and much more from one account. Tracking your money has never been easier.
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
</script>

<style scoped>
.benefits-container {
    background-color: #f3f4f6;
}
.benefits-container > div {
    width: 100%;
    max-width: 1110px;
    margin: auto;
    padding: 96px 0;
}
.benefits-top {
    width: 60%;
    margin-bottom: 32px;
}
.benefits-top h2 {
    color: #2d314d;
    font-weight: 300;
    line-height: 1.15;
    font-size: 1.875rem;
    margin-bottom: 1.5625rem;
}
.benefits-top h3 {
    color: #9698a6;
    font-weight: 300;
    line-height: 1.15;
    font-size: 1.125rem;
    margin-bottom: 2.25rem;
}
.benefits-cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
}
.benefits-card {
    display: flex;
    flex-direction: column;
    gap: 24px;
    padding: 15px;
}
.benefits-card img {
    margin-bottom: 16px;
}
.benefits-card span {
    font-size: 1.25rem;
    color: #2d314d;
    line-height: 1.5rem;
    font-weight: 300;
}
.benefits-card p {
    font-size: 0.875rem;
    color: #9698a6;
    line-height: 1.5;
    font-weight: 300;
    margin: 0;
}

@media(max-width: 1023px) {
    .benefits-top {
        width: 80%;
        margin: 0 auto 32px;
        text-align: center;
    }
    .benefits-top h2 {
        font-size: 2.2rem;
    }
    .benefits-top h3 {
        font-size: 0.9rem;
    }
    .benefits-cards {
        grid-template-columns: repeat(1, 1fr);
        text-align: center;
    }
    .benefits-card {
        padding: 15px 40px;
    }
    .benefits-card img {
        margin: 0 auto 0;
    }
}
</style>