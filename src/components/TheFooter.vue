<script>
    
    export default {
        data() {
            return {
                DcComicsLinks: [
                    { name: "Characters"},
                    { name: "Comics" },
                    { name: "Movies"},
                    { name: "Tv"},
                    { name: "Games"},
                    { name: "Videos"},
                    { name: "News"},
                    ],
                ShopLinks:[
                    { name: "Shop Dc"},
                    { name: "Shop Collectables" },
                    ],
                DCLinks:[
                    { name: "Terms Of Use"},
                    { name: "Privacy Policy(New)" },
                    { name: "AdChoice"},
                    { name: "Advertising"},
                    { name: "Jobs"},
                    { name: "Subscriptions"},
                    { name: "Talent Workshops"},
                    { name: "CPSC Certificates"},
                    { name: "Ratings"},
                    { name: "Shop Help"},
                    { name: "Contact Us"},
                    ],
                SitesLinks:[
                    { name: "DC"},
                    { name: "Mad Magazine"},
                    { name: "DC Kids"},
                    { name: "DC Universe"},
                    { name: "DC Power Visa"},
                    ],

                footerLinks: [
                    { name: "DIGITAL COMICS", img: "buy-comics-digital-comics.png" },
                    { name: "DC MERCHANDISE", img: "buy-comics-merchandise.png" },
                    { name: "SUBSCRIPTION", img: "buy-comics-subscriptions.png" },
                    { name: "COMIC SHOP LOCATOR", img: "buy-comics-shop-locator.png" },
                    { name: "DC POWER VISA", img: "buy-dc-power-visa.svg" },
                ]
                };
        },
    }

</script>

<template> 
    <footer>
        <section class="first-footer container">
            <ul class="d-flex align-items-center justify-content-between">
                <li v-for="link in footerLinks" class="mt-5">
                    <a href="#" class="nav-link text-white">
                        <img v-bind:src="`/src/assets/img/${link.img}`" class="blueImg" alt="" />
                        {{ link.name }}
                    </a>
                </li>
            </ul>
        </section>

        <section class="second-footer">
            <div class="container d-flex">
                <div class="me-5">
                    <h4 class="pt-5">DC COMICS</h4>
                    <div v-for="link in DcComicsLinks">
                        <a href="#">
                            {{ link.name }}
                        </a>
                    </div>

                    <h4 class="pt-2">SHOP</h4>
                    <div v-for="link in ShopLinks">
                        <a href="#">
                            {{ link.name }}
                        </a>
                    </div>
                </div>


                <div class="me-5">
                    <h4 class="pt-5">DC</h4>
                    <div v-for="link in DCLinks">
                        <a href="#">
                            {{ link.name }}
                        </a>
                    </div>
                </div>

                <div>
                    <h4 class="pt-5">SITES</h4>
                    <div class="" v-for="link in SitesLinks">
                        <a href="#">
                            {{ link.name }}
                        </a>
                    </div>
                </div>

                <img src="../assets/img/dc-logo-bg.png" alt="" class="big-logo">
            </div>
        </section>

        <section class="third-footer">
            <div class="container d-flex justify-content-between pt-3">
                <div>
                <button class="button-footer"><strong>SIGN-UP NOW!</strong></button>
                </div>

                <div class="d-flex">
                    <div class="follow me-3"><strong>FOLLOW US</strong></div>
                    <div>
                        <img src="../assets/img/footer-facebook.png" alt="" class="me-3">
                        <img src="../assets/img/footer-twitter.png" alt="" class="me-3">
                        <img src="../assets/img/footer-youtube.png" alt="" class="me-3">
                        <img src="../assets/img/footer-pinterest.png" alt="" class="me-3">
                        <img src="../assets/img/footer-periscope.png" alt="" class="me-3">
                    </div>
                </div>
            </div>
            
        </section>

    </footer>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;
    .first-footer {
        min-height: 160px;

        .blueImg {
        max-height: 70px;
        width: 50px;
        }

        li {
            list-style: none;
        }  
    }
    

    footer {
        height: 170px;
        background-color: $color-primary;

        p {
        color: white;
        }
    }

    .second-footer {
        background-image: url("../assets/img/footer-bg.jpg");
        height: 450px;
        position: relative;
        overflow: hidden;

        h4 {
        color: white;
        }

        
        a {
            color: $color-tertiary;
            list-style: none;
            text-decoration: none;
        }

        .big-logo {
            height: 130%;
            position: absolute;
            right: 200px;
            top: 50%;
            transform: translateY(-50%);
        }
        
    }

    .third-footer {
        background-color: $color-secondary;
        height: 100px;
    }

    .button-footer {
        color: white;
        border: 2px solid $color-primary;
        background-color: $color-secondary;
        padding: 1rem;
    }

    .follow {
        color: $color-primary;
    }
</style>