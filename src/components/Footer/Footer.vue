<template>
    <footer>
        <div class="footer-container">
            <div class="footer-logo-and-social">
                <img class="footer-logo-and-social__logo" src="../../assets/geral/logo-dark.svg" alt="Logo">
                <ul class="footer-social">
                    <li>
                        <a href="">
                            <img src="../../assets/footer/icon-facebook.svg" width="20" height="20" alt="Facebook" />
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../../assets/footer/icon-youtube.svg" width="20" height="20" alt="Youtube" />
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../../assets/footer/icon-twitter.svg" width="20" height="20" alt="Twitter/X" />
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../../assets/footer/icon-pinterest.svg" width="20" height="20" alt="Pinterest" />
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../../assets/footer/icon-instagram.svg" width="20" height="20" alt="Instagram" />
                        </a>
                    </li>
                </ul>
            </div>
            <div>
                <ul class="footer-menu">
                    <li>
                        <a href="">
                            About Us
                        </a>
                    </li>
                    <li>
                        <a href="">
                            Contact
                        </a>
                    </li>
                    <li>
                        <a href="">
                            Blog
                        </a>
                    </li>
                    <li>
                        <a href="">
                            Careers
                        </a>
                    </li>
                    <li>
                        <a href="">
                            Support
                        </a>
                    </li>
                    <li>
                        <a href="">
                            Privacy Policy
                        </a>
                    </li>
                </ul>
            </div>
            <div class="footer-button">
                <button>
                    <a href="">
                        Request Invite
                    </a>
                </button>
                <span>© Easybank. All Rights Reserved</span>
            </div>
        </div>
    </footer>
    <div class="footer-copyright">
        Coded by <a href="">Liniker Brito</a>
    </div>
</template>
<script>
</script>

<style scoped>
footer {
    background-color: #2d314d;
    color: #fff;
    padding: 2.5rem;

}
.footer-container {
    width: 100%;
    max-width: 1110px;
    margin: auto;
    display: flex;
    justify-content: space-between;
}
.footer-logo-and-social {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}
.footer-social {
    list-style: none;
    display: flex;
    gap: 20px;
    padding: 0;
}
.footer-menu {
    display: grid;
  grid-auto-flow: column;
  grid-template-rows: repeat(3, auto);
  grid-auto-columns: minmax(180px, 1fr);
  gap: .5rem 1rem;
  align-content: start;
  list-style-type: none;
  padding: 0;
  margin: 0;
}
.footer-menu a {
    color: #fff;
    text-decoration: none;
    line-height: 2.25;
    font-size: 0.875rem;
    transition: color 300ms ease-in-out;
}
.footer-menu a:hover {
    color: #31d35c;
}
.footer-button {
    display: flex;
    flex-direction: column;
    align-items: end;
    gap: 1.5rem;
    color: #fff;
}
.footer-button > button {
    color: #fff;
    background: linear-gradient(to right, #31d35c, #2bb7da);
    padding: 0.875rem 2.1875rem;
    border-radius: 3.125rem;
    width: fit-content;
}
.footer-button > button > a {
    color: #fff;
    font-size: 0.875rem;
    text-decoration: none;
}
.footer-button > span {
    color: #9698a6;
    font-size: 0.8125rem;
    text-decoration: none;
}
.footer-copyright {
    width: 100%;
    max-width: 1110px;
    margin: auto;
    padding: 1rem 1rem;
    color: #9698a6;
}
@media(max-width: 1023px) {
    .footer-container {
        display: flex;
        flex-direction: column;
    }
    .footer-logo-and-social__logo {
        max-width: 139px;
        margin: auto auto 30px auto;
    }
    .footer-social {
        margin: auto auto 30px auto;
    }
    .footer-menu {
        grid-auto-flow: row;
        grid-template-rows: none;
        grid-template-columns: 1fr;
        grid-auto-columns: unset;
    }
    .footer-menu li {
       text-align: center;
    }
    .footer-button {
        align-items: center;
        margin-top: 30px;
    }
}
</style>