<template>
    <section class="main">
        <div class="container pt-5">
            <div class="row">
                <div class="col-9 offset-3 pb-4">
                    <img src="../assets/artist-quote-icon.png" alt="image">
                </div>
                <div class="col-6 title">
                    <h1>I coach and mentor visual artists, like you, to Create Like You Mean It</h1>
                    <p>Martin Garrix</p>
                </div>
                <div class="col-6 text">
                    <p>As a coach and mentor, my ultimate goal is to motivate visual artist toward inspired action. I help you get you back on track to being the productive, creatice, meaningful and authentic artist you truly want to be. I support artist in crafting and living a creative life as well as feeling good about themselves and their art.
                    </p>
                    <p>As an artist and a educator for nearly 30 years, I understand what it takes to create</p>
                    <button type="button" class="btn btn-text">Get started today</button>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Sec2Main',
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.main {
    height: 500px;
    display: flex;
    .title {
        text-align: center;
        padding: 0 50px;
        h1 {
            font-weight: $font-weight-primary;
        }
        p {
            color: $primary-color-p;
            font-family: $fontFamily;
            overflow: $overflow;
            font-size: $fontsixe-p;
        }
    }
    .text {
        color: $primary-color-text;
        .btn-text {
            background-color: $backgroung-btn;
            color: $color-btn;
            padding: 8px 40px;
            transition: transform .4s;
            border: 1px solid transparent;
            &:hover {
                transform: scale(0.9);
                box-shadow: 0 0 0 2px $color-btn;;
                border: 1px solid white;
            } 
        }
    }
}
</style>