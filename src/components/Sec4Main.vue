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
                        <div class="testimonial">
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
                    job: "/Freelancer",
                },
                {
                    title: "It's a choise of quality for people with special needs",
                    subtitle: "I'm a very strict person so I require everything to be organized and neat. Then, I'll be able to to make things right and shine. MaxCoach guys just got to me.",
                    avatar: require("@/assets/artist-testimonial-avatar-03.jpg"),
                    Name: "Florence Themes",
                    job: "/Multimedia Admin",
                },
                {
                    title: "Professional team of specialist and passionate mentors at reach",
                    subtitle: "I need to get a certification for English profieciency and MaxCosch is my best choise. Their tutors are smart and professional whr dealing whth students",
                    avatar: require("@/assets/artist-testimonial-avatar-02.jpg"),
                    Name: "Madley Pondor",
                    job: "/IT Specialist",
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
.main {
    background-color: #f1efee;
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        p {
            color: #73c6f1;
        }
        h1 {
            font-weight: 900;
        }
        .testimonial {
            background-color: white;
            padding: 30px;
            margin-bottom: 30px;
            h5 {
                color: #424242;
            }
            h6 {
                color: #747474;
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
                        color: #747474;
                        font-size: 12px;
                    }
                }
            }
        }
    }
}
</style>