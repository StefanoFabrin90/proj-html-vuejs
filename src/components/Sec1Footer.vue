<template>
    <section class="footer">
        <img class="poster-right" src="../assets/artist-shape-color-paint-top-left.png" alt="">
        <img class="poster-left" src="../assets/artist-shape-color-paint-bottom-right.png" alt="">
        <div class="container mb-5 mt-5">
            <div class="row">
                <div class="col-4 d-flex text">
                    <h2>Newsletter to get in touch</h2>
                </div>
                <div class="col-8 email">
                    <div class="input-group mb-3 align-items-center textemail">
                        <input type="text" placeholder="Your e-mail">
                        <i class="fas fa-arrow-right"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Sec1Footer',
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.footer {
    background-color: $backgroung-footer;
    position: relative;
    .poster-right {
        position: absolute;
        top: 0;
        height: 100%;
    }
    .poster-left {
        position: absolute;
        bottom: 0;
        right: 0;
        height: 100%;
    }
    .container {
        color: $color-white;
        .text {
            z-index: 1;
            h2 {
                font-size: 3rem;
                text-align: end;
                font-weight: $font-weight-third;
            }
        }
        .email {
            z-index: 1;
            display: flex;
            .textemail {
                padding-left: 20px;
                    &:hover input{
                        border-bottom: 1px solid black;
                    }
                    &:hover i{
                        color: black;
                    }
                input {
                    background-color: $backgroung-footer;
                    color: $color-white;
                    font-size: 25px;
                    width: 80%;
                    height: 35px;
                    border: 0;
                    border-bottom: 1px solid $color-white;
                    outline: none;
                    transition: border .3s;
                    &:focus {
                        border-bottom: 1px solid black;
                    } 
                }
                i {
                    font-size: 25px;
                    &:focus {
                        color: black;
                    } 
                }
            }
        }
    }
}
</style>