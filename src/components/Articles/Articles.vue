<template>
    <section class="articles-container">
        <div>
            <div class="articles-top">
                <h2>Latest Articles</h2>
            </div>
            <div class="articles-cards">
                <div class="article-card">
                    <img src="../../assets/articles/image-currency.jpg" width="243" height="200" alt="currency">
                    <div>
                        <span>By Claire Robinson</span>
                        <h3>Receive money in any currency with no fees</h3>
                        <p>
                            The world is getting smaller and we’re becoming more mobile.So why should you be forced to only receive money in a single.
                        </p>
                    </div>
                </div>
                <div class="article-card">
                    <img src="../../assets/articles/image-restaurant.jpg" width="243" height="200" alt="restaurant">
                    <div>
                        <span>By Wilson Hutton</span>
                        <h3>Treat yourself without worrying about money</h3>
                        <p>
                            Our simple budgeting feature allows you to separate out your spending and set realistic limits each month. That means you

                        </p>
                    </div>
                </div>
                <div class="article-card">
                    <img src="../../assets/articles/image-plane.jpg" width="243" height="200" alt="plane">
                    <div>
                        <span>By Wilson Hutton</span>
                        <h3>Take your Easybank card wherever you go</h3>
                        <p>
                            We want you to enjoy your travels. This is why we don’t charge any fees on purchases while you’re abroad. We’ll even show you
                        </p>
                    </div>
                </div>
                <div class="article-card">
                    <img src="../../assets/articles/image-confetti.jpg" width="243" height="200" alt="confetti">
                    <div>
                        <span>By Claire Robinson</span>
                        <h3>Our invite-only Beta accounts are now live!</h3>
                        <p>
                            After a lot of hard work by the whole team, we’re excited tolaunch our closed beta. It’s easy to request an invite through the site

                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
</script>

<style scoped>
.articles-container {
    background-color: #fafafa;
}
.articles-container > div {
    width: 100%;
    max-width: 1110px;
    margin: auto;
    padding: 96px 0;
}
.articles-top h2 {
    color: #2d314d;
    font-weight: 300;
    line-height: 1.15;
    font-size: 1.875rem;
    margin-bottom: 1.5625rem;
}
.articles-cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1.875rem;
}
.article-card {
    display: flex;
    flex-direction: column;
    box-shadow: 0px 0.1875rem 0.75rem rgba(0, 0, 0, 0.15);
    border-radius: 0.3125rem;
    overflow: hidden;
    transition: all 150ms ease-in-out;
    cursor: pointer;
}
.article-card:hover {
    transform: scale(1.03);
    box-shadow: 0px 0.1875rem 0.8rem rgba(0, 0, 0, 0.25);
}
.article-card img {
    width: 100%;
}
.article-card > div {
    padding: 30px 25px;
}
.article-card > div > span{
    font-size: 0.625rem;
    margin-bottom: 0.75rem;
    color: #9698a6;
}
.article-card > div > h3 {
    font-size: 1.0625rem;
    margin-bottom: 0.5rem;
    color: #2d314d;
    line-height: 1.2;
    font-weight: 300;
}
.article-card > div > p {
    font-size: 0.8125rem;
    color: #9698a6;
    line-height: 1.3;
    font-weight: 300;
}
@media(max-width: 1023px) {
    .articles-container {
        padding: 0 24px;
    }
    .articles-container > div {
        padding: 0;
    }
    .articles-cards {
        grid-template-columns: 1fr;
    }
}
</style>