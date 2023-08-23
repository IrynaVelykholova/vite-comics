<script>
    export default {
    components:{

    }
} 
</script>

<template> 
    <header class="container">
        <img src="../assets/img/dc-logo.png" alt="Logo DC">
        <ul>
            <li><a href="#" class="nav-link">CHARACTERS</a></li>
            <li><a href="#" class="nav-link">COMICS</a></li>
            <li><a href="#" class="nav-link">MOVIES</a></li>
            <li><a href="#" class="nav-link">TV</a></li>
            <li><a href="#" class="nav-link">GAMES</a></li>
            <li><a href="#" class="nav-link">COLLECTIBLES</a></li>
            <li><a href="#" class="nav-link">VIDEOS</a></li>
            <li><a href="#" class="nav-link">FANS</a></li>
            <li><a href="#" class="nav-link">NEWS</a></li>
            <li><a href="#" class="nav-link">SHOP</a></li>
        </ul>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

header {
    display: flex;
    justify-content: space-between;
    height: 130px;

    img {
    width: 100px;
    height: 100px;
    align-self: center;
    }

    ul {
    display: flex;
    align-items: center;
        li {
            list-style: none;
            margin-left: 12px;
        }
    }

    nav-link {
        text-decoration: none;
        color: black;
        &.hover {
            color: $color-primary;
            border-bottom: 2px solid $color-primary;
        }
    }
}








</style>