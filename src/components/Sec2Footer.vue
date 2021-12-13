<template>
    <section class="footer">
        <div class="container mt-5 mb-5">
            <div class="row">
                <div class="col-4 column column-left">
                    <h4>Address</h4>
                    <ul class="information">
                        <li>382 NE 191st St# 87394 Miami, FL 3319-3899</li>
                        <li>+1(305) 547-9909 (9am -5pm EST, Monday -Friday)</li>
                        <li>support@maxcoach.com</li>
                    </ul>
                    <div class="socials">
                        <ul class="item">
                            <li><i class="fab fa-facebook-square"></i></li>
                            <li><i class="fab fa-twitter"></i></li>
                            <li><i class="fab fa-instagram"></i></li>
                            <li><i class="fab fa-linkedin"></i></li>
                        </ul>
                    </div>
                </div>
                <div class="col-4 column column-center">
                    <div class="row">
                        <div class="col-6">
                            <h4>Explore</h4>
                            <ul class="explore">
                                <li>Start here</li>
                                <li>Success story</li>
                                <li>Blog</li>
                                <li>Courses</li>
                                <li>Contact us</li>
                            </ul>
                        </div>
                        <div class="col-6">
                            <h4>Information</h4>
                            <ul class="information">
                                <li>Membership</li>
                                <li>Purchase guide</li>
                                <li>Privacy policy</li>
                                <li>Terms of services</li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-4 column column-right">
                    <h4>Instagram <span>@maxcoach</span></h4>
                    <div class="row">
                        <div class="col-4">
                            <div class="poster">
                                <img src="../assets/artist-event-01-250x300.jpg" alt="">
                            </div>
                        </div>
                        <div class="col-4">
                            <div class="poster">
                                <img src="../assets/artist-event-02-250x300.jpg" alt="">
                            </div>
                        </div>
                        <div class="col-4">
                            <div class="poster">
                                <img src="../assets/artist-event-03-250x300.jpg" alt="">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="text-center copyright">
                <p>	&#169; Maxcoach. All Rights Reserved</p>
            </div>
            <a href="#1">
                <div class="navigation mb-3">
                    <i class="fas fa-long-arrow-alt-up"></i>
                </div> 
            </a>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Sec2Footer',
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.footer {
    position: relative;
}
.container {
    font-weight: $font-weight-third;
    .copyright {
        font-size: 12px;
        padding-top: 100px;
        color: $primary-color-text;
    }
    .column {
        h4 {
            padding-bottom: 1rem;
            color: $color-black;
            font-weight: 700;
        }
    }
    .column-left {
        .information {
            padding-left: 0;
            li {
                padding: 5px 0px;
                color: $primary-color-text;
                cursor: pointer;
                &:hover {
                    text-decoration: underline;
                }
            }
        }
        .item {
            list-style: none;
            display: flex;
            padding-left: 0;
            li {
                padding: 10px 40px 10px 0px;
                font-size: 30px;
                cursor: pointer;
                color: $primary-color-text;
            }
        }
    }
    .column-center {
        ul {
            padding-left: 0;
            li {
                padding: 5px 0px;
                cursor: pointer;
                color: $primary-color-text;
                &:hover {
                    text-decoration: underline;
                }
            }
        }
    }
    .column-right {
        .poster {
            width: 150px;
            height: 150px;
            img {
                width: 100%;
            }
        }
        h4 {
            span {
                color: $color-btn;
                font-size: 16px;
                vertical-align: middle;
            }
        }
    }
    a {
        color: $color-white;
    }
    .navigation {
        position: absolute;
        bottom: 0;
        right: 50px;
        width: 40px;
        height: 40px;
        text-align: center;
        line-height: 40px;
        background-color: $color-btn;
        border-radius: 50%;
        cursor: pointer;
        i {
            vertical-align: middle;
        }
    }
}
</style>