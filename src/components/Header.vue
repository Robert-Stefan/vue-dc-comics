<template>
    <header>
        <a href="/">
            <img src="../assets/img/dc-logo.png" alt="logo">
        </a>

        <!--nav items-->
        <nav>
            <ul>
                <li><a href="/">Characters</a></li>
                <li><a href="/">Characters</a></li>
                <li><a href="/">Characters</a></li>
                <li><a href="/">Characters</a></li>
                <li><a href="/">Characters</a></li>
                <li><a href="/">Characters</a></li>
                <li><a href="/">Characters</a></li>
                <li><a href="/">Characters</a></li>
                <li><a href="/">Characters</a></li>
                <li><a href="/">Characters</a></li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'Header',
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
    margin: 3rem 1rem;
}

li a {
    padding: 1rem;
    text-decoration: none;
    padding-bottom: 2rem;
}

li a:hover {
  border-bottom: 3px solid blue;
}

</style>