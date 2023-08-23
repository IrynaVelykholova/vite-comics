<script>
    
    export default {
    components:{

    }
} 
</script>

<template> 
    <footer>
        <section class="first-footer container">
            <div class="d-flex align-items-center mt-3">
                <div><img src="../assets/img/buy-comics-digital-comics.png" alt=""></div>
                <p class="ms-2">DIGITAL COMICS</p>
            </div>
            
            <div class="d-flex align-items-center mt-3">
                <div><img src="../assets/img/buy-comics-merchandise.png" alt=""></div>
                <p class="ms-2">DC MERCHANDISE</p>
            </div>

            <div class="d-flex align-items-center mt-3">
                <div><img src="../assets/img/buy-comics-subscriptions.png" alt=""></div>
                <p class="ms-2">SUBSCRIPTION</p>
            </div>

            <div class="d-flex align-items-center mt-3">
                <div><img src="../assets/img/buy-comics-shop-locator.png" alt=""></div>
                <p class="ms-2">COMIC SHOP LOCATOR</p>
            </div>

            <div class="d-flex align-items-center mt-3">
                <div><img src="../assets/img/buy-dc-power-visa.svg" alt=""></div>
                <p class="ms-2">DC POWER VISA</p>
            </div>
        </section>

        <section class="second-footer">
            <div class="container d-flex">
                <div class="me-5">
                    <h3 class="pt-5">DC COMICS</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>

                    <h3 class="pt-2">SHOP</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                    </ul>
                </div>

                <div class="me-5">
                    <h3 class="pt-5">DC</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                </div>

                <div>
                    <h3 class="pt-5">SITES</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                    </ul>
                </div>
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
        display: flex;
        justify-content: space-between;

        img {
        width: 80px;
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

        h3 {
        color: white;
        }

        ul {
            li {
                color: $color-tertiary;
                list-style: none;
                margin-left: -2rem;
            }
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