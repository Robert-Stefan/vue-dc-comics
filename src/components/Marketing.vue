<template>
  <div class="container">
      <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.url">
                <img :src="link.img" :alt="link.text">
                <span>{{ link.text }}</span>
            </a>  
          </li> 
      </ul>
  </div>
</template>

<script>
export default {
    name: 'Marketing',
    data() {
        return {
            links: [
                {
                    text: 'Digital Comics',
                    url: '/digitalcomics',
                    img: require('../assets/img/buy-comics-digital-comics.png'),
                },
                {
                    text: 'DC Merchandise',
                    url: '/dcmerchandise',
                    img: require('../assets/img/buy-comics-merchandise.png'),
                },
                {
                    text: 'Subscription',
                    url: '/subscription',
                    img: require('../assets/img/buy-comics-subscriptions.png'),
                },
                {
                    text: 'Comic Shop Locator',
                    url: '/comicshoplocator',
                    img: require('../assets/img/buy-comics-shop-locator.png'),
                },
                {
                    text: 'DC Power Visa',
                    url: '/dcpowervisa',
                    img: require('../assets/img/buy-dc-power-visa.svg'),
                },
            ]
        }
    }
}
</script>

<style scoped>

.container {
    height: 165px;
    background: #0482f9;
}

ul {
    display: flex;
    justify-content: center;
    padding-top: 3rem;
}

li {
    list-style: none;
}

img {
    width: 60px;
    padding-right: 10px;
}

img:nth-child(4) {
    width: 40px;
}

li a {
    display: flex;
    align-items: center;
    padding: 0 55px;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 15px;
    color: #fff;
}
</style>