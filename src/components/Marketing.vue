<template>
  <div class="container">
      <ul>
          <li>
            <a href="#">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>Digital Comics</span>
            </a>  
          </li>
         <li>
            <a href="#">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>Digital Comics</span>
            </a>  
          </li>
          <li>
            <a href="#">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>Digital Comics</span>
            </a>  
          </li>
          <li>
            <a href="#">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>Digital Comics</span>
            </a>  
          </li>
          <li>
            <a href="#">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>Digital Comics</span>
            </a>  
          </li>
      </ul>
  </div>
</template>

<script>
export default {
    name: 'Marketing',
}
</script>

<style scoped>

.container {
    height: 175px;
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