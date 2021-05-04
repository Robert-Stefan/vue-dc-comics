<template>
  <div class="container">
      <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.url">
                <img :src="`@/assets/img/${link.img}.png`" :alt="link.text">
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
                    img: 'buy-comics-digital-comics',
                },
                {
                    text: 'DC Merchandise',
                    url: '/dcmerchandise',
                    img: 'buy-comics-merchandise',
                },
                {
                    text: 'Subscription',
                    url: '/subscription',
                    img: 'buy-comics-subscriptions',
                },
                {
                    text: 'Comic Shop Locator',
                    url: '/comicshoplocator',
                    img: 'buy-comics-shop-locator',
                },
                {
                    text: 'DC Power Visa',
                    url: '/dcpowervisa',
                    img: 'buy-dc-power-visa',
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