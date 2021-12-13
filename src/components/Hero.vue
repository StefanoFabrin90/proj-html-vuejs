<template>
    <section class="hero">
        <div class="column-right">
            <!-- <img src="../assets/artist-shape-02.png" alt=""> -->
            <img class="first" src="../assets/artist-hero-image-01.jpg" alt="">
            <img class="second" src="../assets/artist-hero-image-02.jpg" alt="">
            <img class="third" src="../assets/artist-hero-image-03.png" alt="">
            <img class="fourth" src="../assets/artist-shape-03.png" alt="">
        </div>
        <div class="column-center">
            <p>Hello, I'm Matin</p>
            <h2>Artist Coaching And Mentoring Might Be for You.</h2>
            <button type="button" class="btn btnHero">Get started today</button>
        </div>
        <div class="column-left">
            <!-- <img class="first" src="../assets/artist-shape-01.png" alt=""> -->
            <img class="second" src="../assets/artist-shape-04.png" alt="">
            <img class="third" src="../assets/artist-hero-image-04.jpg" alt="">
            <img class="fourth" src="../assets/artist-shape-05.png" alt="">
        </div>
    </section>
</template>

<script>
export default {
    name:'Hero',
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.hero {
    height: 400px;
    background-color:$backgroung-hero;
    display: flex;
    position: relative;
    .column-right {
        width: calc(100% / 3);
        background-image: url('../assets/artist-shape-02.png');
        background-repeat: no-repeat;
        background-size: contain;
        .first {
            position: absolute;
            width: 120px;
            bottom: 20px;
            left: 205px;
            z-index: 2;
        }
        .second {
            width: 180px;
            position: absolute;
            top: 30px;
            left: 320px;
            z-index: 1;
        }
        .third {
            width: 120px;
            position: absolute;
            bottom: 20px;
            left: 450px;
        }
        .fourth {
            width: 200px;
            position: absolute;
            top: 50px;
            left: 125px;
        }
    }
    .column-center {
        width: calc(100% / 3);
        text-align: center;
        font-weight: 900;
        padding: 0 80px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        p {
            color: $primary-color-p;
            font-family: $fontFamily;
            overflow: hidden;
            font-size: 3rem;
        }
        .btnHero {
            padding: 8px 40px;
            background-color: $color-btn;
            color: $color-white;
            margin-top: 20px;
            transition: transform .4s;
            border: 1px solid transparent;
            &:hover {
                transform: scale(0.9);
                box-shadow: 0 0 0 2px $color-btn;;
                border: 1px solid white;
            } 
        }
    }
    .column-left {
        width: calc(100% / 3);
        background-image: url('../assets/artist-shape-01.png');
        background-repeat: no-repeat;
        background-size: contain;
        .second {
            width: 65px;
            position: absolute;
            top: 40px;
            right: 200px;
        }
        .third {
            width: 160px;
            position: absolute;
            bottom: 20px;
            right: 260px;
            z-index: 1;
        }
        .fourth {
            width: 250px;
            position: absolute;
            bottom: 0;
            right: 135px;
        }
    }
}
</style>