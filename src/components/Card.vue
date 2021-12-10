<template>
    <div class="card h-100 p-3">
        <img :src="image" :alt="title">
        <div class="p-3">
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
.card {
    border: none;
    p {
        color: #f07c44;
    }
    i, span {
        color: #595959;
        padding: 10px 10px 0px 0px;
    }
}
</style>