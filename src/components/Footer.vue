<template>
    <footer>
        <div class="footer-top">
            <div class="container">
                <div class="links">
                    <div class="first-column">
                        <h2>Dc Comics</h2>
                        <ul>
                            <li
                                v-for="(link, index) in dcComics"
                                :key="index"
                            >
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                        <h2>Shop</h2>
                        <ul>
                            <li
                                v-for="(link, index) in shop"
                                :key="index"
                            >
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="second-column">
                        <h2>DC</h2>
                        <ul>
                            <li
                                v-for="(link, index) in dc"
                                :key="index"
                            >
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h2>Sites</h2>
                        <ul>
                            <li
                                v-for="(link, index) in sites"
                                :key="index"
                            >
                                <a :href="link.url">{{ link.text }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="Logo BG">
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container">
                <div class="button">
                    Sign-up now!
                </div>

                <div class="socials">
                    <h2 class="color">follow us</h2>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            dcComics: [
                {
                    text: 'Characters',
                    url: '/characters',
                },
                {
                    text: 'Comics',
                    url: '/comics',
                },
                {
                    text: 'Movies',
                    url: '/movies',
                },
                {
                    text: 'TV',
                    url: '/tv',
                },
                {
                    text: 'Games',
                    url: '/games',
                },
                {
                    text: 'Videos',
                    url: '/videos',
                },
                {
                    text: 'News',
                    url: '/news',
                },
            ],
            shop: [
                {
                    text: 'Shop DC',
                    url: '/shopdc',
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '/shopdccollectibles',
                },
            ],
            dc: [
                {
                    text: 'Terms Of Use',
                    url: '/termsofuse',
                },
                {
                    text: 'Privacy policy (New)',
                    url: '/privacypolicy',
                },
                {
                    text: 'Ad Choices',
                    url: '/adchoices',
                },
                {
                    text: 'Advertising',
                    url: '/advertising',
                },
                {
                    text: 'Jobs',
                    url: '/jobs',
                },
                {
                    text: 'Subscriptions',
                    url: '/subscriptions',
                },
                {
                    text: 'Talent Workshops',
                    url: '/talentworkshops',
                },
                {
                    text: 'CPSC Certificates',
                    url: '/cpsccertificates',
                },
                {
                    text: 'Ratings',
                    url: '/ratings',
                },
                {
                    text: 'Shop Help',
                    url: '/shophelp',
                },
                {
                    text: 'Contact Us',
                    url: '/contactus',
                },
            ],
            sites: [
                {
                    text: 'DC',
                    url: '/dc',
                },
                {
                    text: 'MAD Magazine',
                    url: '/madmagazine',
                },
                {
                    text: 'DC Kids',
                    url: '/dckids',
                },
                {
                    text: 'DC Universe',
                    url: '/dcuniverse',
                },
                {
                    text: 'DC Power Visa',
                    url: '/dcpowervisa',
                },
            ],
        }
    }
}
</script>

<style scoped>

.footer-top {
    background-image: url(../assets/img/footer-bg.jpg);
}

.container {
    display: flex;
    justify-content: space-between;
    width: 70%;
    margin: 0 auto;
    padding: 3rem 0;
    overflow: hidden;
}

.links {
    display: flex;
}

.logo img {
    transform: translateY(-140px)
}


.logo {
    height: 280px;
}

.first-column,
.second-column {
    margin-right: 2rem;
}

h2 {
    text-transform: uppercase;
    font-weight: bold;
    color: #fff;
}

ul {
    padding: 1rem 0;
    list-style: none;
}

ul li a {
    text-decoration: none;
    color: #859595;
    line-height: 22px;
    font-size: 14px;
}

ul li a:hover {
    color: #fff;
}

.footer-bottom {
    background-color: #303030
}

.button {
    font-size: 22px;
    padding: 15px;
    border: 3px solid #0482f9;
    color: #fff;
    text-transform: uppercase;
    cursor: pointer;
}

.color {
    margin-right: 20px;
    color: #0482f9;
}

.footer-bottom img {
    padding: 10px;
    cursor: pointer;
}

.socials {
    display: flex;
    align-items: center;
}

</style>