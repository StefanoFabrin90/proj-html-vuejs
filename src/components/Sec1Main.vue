<template>
    <section class="main">
        <div class="text">
            <p>Artist Coaching</p>
            <h1>I understand what it takes to create. <br> I can help you with</h1>
        </div>
        <div class="cardList">
            <ul class="listCoaching">
                <li 
                    v-for="(item, index) in cardImage" :key="`item-${index}`"
                >
                    <img :src="item.image" alt="">
                    <h4> {{ item.title }}</h4>
                    <h5> {{ item.subTitle }}</h5>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Sec1Main',
    data() {
        return {
            cardImage: [
                {
                    image: require('@/assets/artist-box-image-01.png'),
                    title: 'Online Course',
                    subTitle: 'Online at coaching now offers you a very powerful way to redesign your artist mind.',
                },
                {
                    image: require('@/assets/artist-box-image-02.png'),
                    title: 'One to One',
                    subTitle: 'Getting the necessary clarity about the current to help you improve your ability.',
                },
                {
                    image: require('@/assets/artist-box-image-03.png'),
                    title: 'Anywhere',
                    subTitle: 'Access to valuable and portable program which you setup and live anywhere you want.',
                },
                {
                    image: require('@/assets/artist-box-image-04.png'),
                    title: 'On Time',
                    subTitle: "Punctuality is our top priority because it's an essetial criteria to acces a program quality.",
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.main {
    height: 500px;
    background-image: url('../assets/maxcoach-shape-14-768x172.png');
    background-repeat: no-repeat;
    background-size: 100%;
    background-position: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    
    .text {
        text-align: center;
        p {
        color: $primary-color-p;
        font-family: $fontFamily;
        overflow: $overflow;
        font-size: $fontsixe-p;
        }
    }
    
    .cardList {
        .listCoaching {
            display: flex;
            justify-content: center;
            list-style: none;
            li {
                width: calc(100% / 5);
                padding: 10px 20px;
                h4 {
                    padding: 10px 0;
                }
                h5 {
                    font-size: 18px;
                    font-weight: $font-weight-third
                }
            }
        }
    }
}
</style>