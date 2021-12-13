<template>
    <section class="main">
        <div class="container">
            <div class="title text-center mt-5 mb-5">
                <p>Upcoming Events</p>
                <h2>Let's Work Together</h2>
            </div>
            <div class="content mb-5">
                <div class="row">
                    <div class="col-6 d-flex mb-5">
                        <div class="poster">
                            <img src="../assets/artist-event-04-250x300.jpg" alt="">
                        </div>
                        <div class="text">
                            <p>NOV 22, 2020</p>
                            <h5>Storytelling Workshop</h5>
                            <p><i class="fas fa-map-marker-alt"></i>  Texas, US</p>
                        </div>
                    </div>
                    <div class="col-6 d-flex mb-5">
                        <div class="poster">
                            <img src="../assets/artist-event-03-250x300.jpg" alt="">
                        </div>
                        <div class="text">
                            <p>OCT 10, 2020</p>
                            <h5>Painting Art Contest 2020</h5>
                            <p><i class="fas fa-map-marker-alt"></i>  New York, US</p>
                        </div>
                    </div>
                    <div class="col-6 d-flex mb-5">
                        <div class="text text-end">
                            <p>NOV 23, 2020</p>
                            <h5>International Art Fair 2020</h5>
                            <p><i class="fas fa-map-marker-alt"></i>  Hamburg, Germany</p>
                        </div>
                        <div class="poster">
                            <img src="../assets/artist-event-02-250x300.jpg" alt="">
                        </div>
                    </div>
                    <div class="col-6 d-flex mb-5">
                        <div class="text text-end">
                            <p>DEC 15, 2020</p>
                            <h5>Street Performance: Call for Artist</h5>
                            <p><i class="fas fa-map-marker-alt"></i>  Illinois, US</p>
                        </div>
                        <div class="poster">
                            <img src="../assets/artist-event-01-250x300.jpg" alt="">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'Sec7Main',
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.container {
    display: flex;
    flex-direction: column;
    align-items: center;
    .title {
        p {
            color: $primary-color-p;
            font-family: $fontFamily;
            overflow: $overflow;
            font-size: $fontsixe-p;
        }
        h2 {
            font-weight: $font-weight-primary;
        }
    }
    .content {
        p {
            color: $primary-color-text;
        }
        .text {
            display: flex;
            flex-direction: column;
            justify-content: center;
            margin: 0px 50px;
        }
    }
}
</style>