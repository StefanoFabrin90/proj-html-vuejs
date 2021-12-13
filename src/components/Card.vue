<template>
    <div class="card h-100 p-3">
        <img :src="image" :alt="title">
        <div class="p-3 itemCard">
            <p> {{ textOne }} </p>
            <h5> {{ title }} </h5>
            <div class="d-flex item-text">
                <div class="d-flex align-items-baseline">
                    <i class="fas fa-file-alt"></i>
                    <span> {{ textTwo }} </span>
                </div>
                <div class="d-flex align-items-baseline">
                    <i class="fas fa-user p"></i>
                    <span> {{ textThree }} </span>
                </div>
            </div>
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
    .item-text {
        padding: 10px 3px 0px 0px;
        i {
            padding-right: 3px;
        }
    }
    .itemCard {
        border: 1px solid transparent;
        &:hover {
            border: 1px solid $color-btn;
            background-color: $color-white;
            position: absolute;
            bottom: 60px;
            width: 85%;
        }
    }
}
</style>