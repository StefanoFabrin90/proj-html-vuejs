<template>
    <div class="card h-100 p-3">
        <img :src="image" :alt="title">
        <div class="p-3 itemCard">
            <p> {{ textOne }} </p>
            <h5> {{ title }} </h5>
            <i class="fas fa-file-alt"></i><span> {{ textTwo }} </span>
            <i class="fas fa-user"></i><span> {{ textThree }} </span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        image: String,
        textOne: String,
        title: String,
        textTwo: String,
        textThree: String,
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.card {
    border: none;
    position: relative;
    p {
        color: $color-btn;
    }
    i, span {
        color: $primary-color-text;
        padding: 10px 10px 0px 0px;
    }
    .itemCard {
        border: 1px solid transparent;
        &:hover {
            border: 1px solid $color-btn;
            background-color: $color-white;
            position: absolute;
            bottom: 50px;
            width: 80%;
        }
    }
}
</style>