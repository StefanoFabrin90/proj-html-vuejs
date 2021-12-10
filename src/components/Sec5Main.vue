<template>
    <section class="main">
        <div class="container mt-5">
            <div class="title text-center mb-5">
                <p>Artist Coaching</p>
                <h2>Latest Online Courses</h2>
            </div>
            <div class="cardList">
                <div class="row">
                    <div class="col-3 mb-3 poster" v-for="(item, index) in cardArtist" :key="`item-${index}`">
                        <!-- card -->
                        <Card 
                            :image="item.image"
                            :textOne="item.price"
                            :title="item.title"
                            :textTwo="item.lesson" 
                            :textThree="item.students"
                        />
                    </div>
                </div>
            </div>
            <div class="mb-5">
                <button type="button" class="btn button">View all course <i class="fas fa-long-arrow-alt-right align-middle"></i></button>
            </div>
        </div>
    </section>
</template>

<script>
import Card from '@/components/Card.vue';
export default {
    name: 'Sec5Main',
    components: {
        Card,
    },
    data() {
        return {
            cardArtist: [
                {
                    image:require('@/assets/artist-course-08-480x480.jpg'),
                    price:"$18.00",
                    title:"The Acrylic Painting academy",
                    lesson: "4 Lessons",
                    students: "50 Studets",
                },
                {
                    image:require('@/assets/artist-course-07-480x480.jpg'),
                    price:"$21.00",
                    title:"Drawing and Shading Complete Course",
                    lesson: "4 Lessons",
                    students: "50 Studets",
                },
                {
                    image:require('@/assets/artist-course-06-480x480.jpg'),
                    price:"$19.00",
                    title:"The Color theory for Digital Aritist",
                    lesson: "7 Lessons",
                    students: "50 Studets",
                },
                {
                    image:require('@/assets/artist-course-05-480x480.jpg'),
                    price:"$35.00",
                    title:"Ultimate Guide to Digital Sketching for Beginner",
                    lesson: "14 Lessons",
                    students: "50 Studets",
                },
                {
                    image:require('@/assets/artist-course-04-480x480.jpg'),
                    price:"$19.00",
                    title:"Portrait Drawing the Smart Way",
                    lesson: "21 Lessons",
                    students: "50 Studets",
                },
                {
                    image:require('@/assets/artist-course-03-480x480.jpg'),
                    price:"$19.00",
                    title:"Mastering Watercolor Painting from Beginner",
                    lesson: "9 Lessons",
                    students: "50 Studets",
                },
                {
                    image:require('@/assets/artist-course-02-480x480.jpg'),
                    price:"$25.00",
                    title:"The Art & Science of Drawing",
                    lesson: "4 Lessons",
                    students: "50 Studets",
                },
                {
                    image:require('@/assets/artist-course-01-480x480.jpg'),
                    price:"$22.00",
                    title:"The Colored Pencil Drawing Course",
                    lesson: "6 Lessons",
                    students: "50 Studets",
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
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
    .button {
        background-color: #fdf0ea;
        color: #ef793f;
        padding: 8px 40px;
    }
}
</style>