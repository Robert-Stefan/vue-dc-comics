<template>
    <header>

        <!--LOGO-->
        <a href="/">
            <img src="../assets/img/dc-logo.png" alt="logo">
        </a>

        <!--nav items-->
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :class="{active: link.current}" :href="link.url">{{ link.text }}</a>
                </li>
                
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            links: [
                { text: 'Characters', url: '/characters', current: false},
                { text: 'Comics', url: '/comics', current: true},
                { text: 'Movies', url: '/movies', current: false},
                { text: 'TV', url: '/tv', current: false},
                { text: 'Games', url: '/games', current: false},
                { text: 'Collectibles', url: '/collectibles', current: false},
                { text: 'Videos', url: '/videos', current: false},
                { text: 'Fans', url: '/fans', current: false},
                { text: 'News', url: '/news', current: false},
                { text: 'Shop', url: '/shop', current: false},
            ]
        }
    }
}
</script>

<style scoped>

header {
    display: flex;
    justify-content: space-around;
    padding-top: 20px;
    text-align: center;
}

ul {
    display: flex;
    justify-content: center;
    list-style: none;
    margin: 0 1rem;
    margin-top: 3rem;
}

li a {
    padding: 1rem;
    font-size: 15px;
    text-decoration: none;
    padding-bottom: 2.1rem;
    text-transform: uppercase;
    font-weight: bold;
    color: rgba(0, 0, 0, 0.726);
}

li a.active,
li a:hover {
    color: #0e92f0;
    border-bottom: 3px solid #0e92f0;
}

img {
    width: 100px;
    padding: 10px;
}

</style>