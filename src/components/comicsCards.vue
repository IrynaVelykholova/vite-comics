<script>
    export default {

        props: {
            imgSrc: String,
            series: String,
            type: String,
            price: Number,
        }
    }
</script>

<template>
        <div class="card border-0 h-100"> 
            <img class="position-relative cards-img" :src="imgSrc" alt="" />

            <div class="card-body text-white bg-black">
                {{ series }}
            </div>

            <div>
                <div class="position-absolute attributes top"> Type: 
                    <br> {{ type }} </div>

                <div class="position-absolute attributes bottom"> Price: {{ price }} </div>
            </div>
        </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.top{
    top: 0;
    background-color: rgba(0, 0, 0, 0.650);
}
.attributes {
    position: absolute;
    width: 100%;
    color: white;
    padding: 1rem 0;
    display: none;
}
.bottom{
    bottom: 28%;
    background-color: rgba(0, 0, 0, 0.650);
}
.card:hover .attributes{
    display: block;
}
.cards-img {
    width: 100%;
    height: 200px;
    aspect-ratio: 1/1;
}
</style>