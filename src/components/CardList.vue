<script>
import axios from 'axios';
export default {
    name: 'CardList',
}
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-12 col-sm-6 col-lg-4">
                <div class="card">
                    <img class="img" :src="card.card_images[0].image_url" alt="">
                    <h3>{{ card.name }}</h3>
                    <div class="textCard">
                        {{ card.archetype }}
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>



<style scoped>
.card {
    background-color: white;

    &:hover {
        filter: drop-shadow(0 0 15px violet);
    }
}

.img {
    width: 100%;
}
</style>
