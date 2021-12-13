<template>
    <section class="main">
        <div class="container">
            <div class="row">
                <div class="col-12 poster">
                    <img src="../assets/artist-video-poster.jpg" alt="">
                </div>
                <div class="col-12 play">
                    <img src="../assets/icon-youtube-play.png" alt="">
                </div>
                <div class="col-12 circle-right">
                    <img src="../assets/maxcoach-shape-05.png" alt="">
                </div>
                <div class="col-12 circle-left">
                    <img src="../assets/maxcoach-shape-05.png" alt="">
                </div>
            </div>
        </div>
        <svg class="waves" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#f5f5f5" fill-opacity="1" d="M0,32L48,48C96,64,192,96,288,133.3C384,171,480,213,576,208C672,203,768,149,864,133.3C960,117,1056,139,1152,133.3C1248,128,1344,96,1392,80L1440,64L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>
    </section>
</template>

<script>
export default {
    name: 'Sec3Main',
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.main {
    position: relative;
    padding-bottom: 100px;
    .row {
        position: relative;
        z-index: 1;
    }
    .poster {
        display: flex;
        justify-content: center;
        z-index: 1;
    }
    .play {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-5%, -50%);
        z-index: 2;
    }
    .circle-right {
        position: absolute;
        top: 0px;
        left: 100px;
    }
    .circle-left {
        img {
            position: absolute;
            bottom: 0px;
            right: 50px;
        }
    }
    .waves {
        position: absolute;
        bottom: 0px;
        right: 0;
    }
}
</style>