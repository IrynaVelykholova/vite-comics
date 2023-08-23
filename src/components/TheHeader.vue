<script>
    export default {
        data() {
            return {
                navLinks: [
                    { name: "CHARACTERS" },
                    { name: "COMICS"},
                    { name: "MOVIES"},
                    { name: "TV" },
                    { name: "GAMES" },
                    { name: "COLLECTABLES" },
                    { name: "VIDEOS" },
                    { name: "FANS" },
                    { name: "NEWS" },
                    { name: "SHOP" },
                ],
            };
        },

    
} 
</script>

<template> 
    <header class="container">
        <img src="../assets/img/dc-logo.png" alt="Logo DC">
        <div class="d-flex align-items-center">
            <div class="ms-3" v-for="link in navLinks"> 
                <a href="#" class="nav-link">
                    {{ link.name }}
                </a>
            </div>
        </div>
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