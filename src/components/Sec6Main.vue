<template>
    <section class="main">
        <div class="container mt-5 mb-5">
            <div class="title text-center mb-5">
                <p>Article and Tips</p>
                <h2>Let's Work Together</h2>
            </div>
            <div class="d-flex">
                <div class="cardItem">
                    <div class="item">
                        <div class="poster">
                            <img src="../assets/artist-blog-03-480x356.jpeg" alt="">
                        </div>
                        <div class="text">
                            <p>Artist</p>
                            <h5>Brush Strokes Energize Trees in Paintings</h5>
                            <div class="d-flex align-items-baseline calendar">
                                <i class="far fa-calendar"></i><span>May 15, 2020</span>
                                <i class="far fa-eye"></i><span>688 views</span>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="cardItem column-central">
                    <div class="text">
                        <p>Artist</p>
                        <h5>Coonection Between Self-Portraits and Identity</h5>
                        <div class="d-flex align-items-baseline calendar">
                            <i class="far fa-calendar"></i><span>May 15, 2020</span>
                            <i class="far fa-eye"></i><span>688 views</span>
                        </div>
                    </div>
                </div>
                <div class="cardItem">
                    <div class="item item-right">
                        <div class="poster">
                            <img src="../assets/artist-blog-01-480x356.jpg" alt="">
                        </div>
                        <div class="text">
                            <p>Artist</p>
                            <h5>Pocket-Sikez Notebooks Hold Miniature Paintings</h5>
                            <div class="d-flex align-items-baseline calendar">
                                <i class="far fa-calendar"></i><span>May 15, 2020</span>
                                <i class="far fa-eye"></i><span>688 views</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Sec6Main',
}
</script>

<style scoped lang="scss">
.main {
    background-color: #f5f7fa;
    background-image: url('../assets/maxcoach-shape-03.png');
    background-repeat: no-repeat;
    background-size: 100%;
    background-position: center;
}
.container {
    display: flex;
    flex-direction: column;
    align-items: center;
    .title {
        p {
            color: #73c6f1;
        }
        h2 {
            font-weight: 900;
        }
    }
    .cardItem {
        height: 500px;
        width: 350px;
        //border: 1px solid black;
        position: relative;
        p {
            text-transform: uppercase;
        }
        i, span {
                padding: 10px 10px 0px 0px;
            }
        .item {
            width: 300px;
            position: absolute;
            bottom: 50px;
            p, .calendar {
               color: lightgray; 
            }
            .text {
                background-color: white;
                padding: 15px;
            }
            .poster {
                img {
                    width: 100%;
                }
            }
        }
        .item-right {
           position: absolute;
           right: 0;
           top: 20px; 
        }
    }
    .column-central {
        background-image: url('../assets/artist-blog-02-500x680.jpg');
        background-size: cover;
        position: relative;
        .text {
            position: absolute;
            bottom: 0;
            color: white;
            padding: 10px;
        }
    }
}
</style>