<template>
    <section class="main">
        <div class="container">
            <div class="title text-center mb-5">
                <p>Testimonilas</p>
                <h1>Why do people love me?</h1>
            </div>
            <div class="cardTestimonial">
                <div class="row">
                    <div class="col-4" v-for="(item, index) in cardTestimonials" :key="`item-${index}`">
                        <div 
                            class="testimonial"
                            :class="{active: index === activeSlide}"
                        >
                            <h5>{{item.title}}</h5>
                            <h6>{{item.subtitle}}</h6>
                            <div class="information">
                                <div class="avatar">
                                    <img width="100px" :src="item.avatar" alt="">
                                </div>
                                <div class="people">
                                    <span>{{item.Name}}</span>
                                    <span class="job">{{item.job}}</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="mb-5 circle">
                <i class="fas fa-arrow-left" @click="prevSlide"></i>
                <i class="fas fa-arrow-right" @click="nextSlide"></i>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Sec4Main',
    data() {
        return {
            cardTestimonials: [
                {
                    title: "High level of efficiency and scientific teaching methods",
                    subtitle: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
                    avatar: require("@/assets/artist-testimonial-avatar-04.jpg"),
                    Name: "Mina Hollance",
                    job: "/ Freelancer",
                },
                {
                    title: "It's a choice of quality for people with special needs",
                    subtitle: "I'm a very strict person so I require everything to be organized and neat. Then, I'll be able to to make things right and shine. MaxCoach guys just got to me.",
                    avatar: require("@/assets/artist-testimonial-avatar-03.jpg"),
                    Name: "Florence Themes",
                    job: "/ Multimedia Admin",
                },
                {
                    title: "Professional team of specialist and passionate mentors at reach",
                    subtitle: "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing whith students",
                    avatar: require("@/assets/artist-testimonial-avatar-02.jpg"),
                    Name: "Madley Pondor",
                    job: "/ IT Specialist",
                },
            ],
            activeSlide: 0,
        }
    },
    methods: {
        prevSlide() {
            this.activeSlide--;

            if (this.activeSlide < 0) {
                this.activeSlide = this.cardTestimonials.length -1;
            }
        },
        nextSlide () {
            this.activeSlide++;

            if (this.activeSlide > this.cardTestimonials.length -1) {
                this.activeSlide = 0;
            }
        }
    },
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.main {
    background-color: $backgroung-header;
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        p {
            color: $primary-color-p;
            font-family: $fontFamily;
            overflow: $overflow;
            font-size: $fontsixe-p;
        }
        h1 {
            font-weight: $font-weight-primary;
        }
        .testimonial {
            background-color: white;
            box-shadow: 0 15px 10px -10px rgba(0,0,0, .2);
            padding: 30px;
            margin-bottom: 30px;
            opacity: 0.2;
            h5 {
                color: $color-black;
            }
            h6 {
                color: $primary-color-text;
                padding: 5px 0;
            }
            .information {
                display: flex;
                .avatar{
                    img {
                        border-radius: 50%;
                }   }
                .people {
                    display: flex;
                    flex-direction: column;
                    justify-content: center;
                    margin-left: 10px;
                    .job {
                        color: $primary-color-text;
                        font-size: 12px;
                    }
                }
            }
        }
        .active {
            opacity: 1;
        }
        .circle {
            i {
                color:$primary-color-text;
                font-size: 20px;
                padding: 10px;
                border: 1px solid $primary-color-text;
                border-radius: 50%;
                margin-right: 15px;
                cursor: pointer;
                &:hover {
                    color: $color-black;
                    border: 1px solid $color-black;
                }
            }
        }
    }
}
</style>