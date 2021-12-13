<template>
    <section class="time">
        <div class="container d-flex header align-items-baseline">
            <div class="text"> 
                <p>Starts <span>tomorrow!</span> Our biggest event of the year...</p> 
            </div>
            <div class="d-flex align-items-baseline">
                <i class="far fa-clock"></i>
                <p class="clock">
                    {{ dateNow }}
                    <span>{{dateDays}}</span>
                </p>
                <button type="button" class="btn geticket">Get ticket</button>
            </div>
        </div>
    </section>
</template>

<script>
import dayjs from 'dayjs';
export default {
    name: 'Sec1Header',
    data() {
        return {
            dateNow: '',
            dateDays: '',
        }
    },
    created(){
        this.createDate();
    },
    methods: {
        createDate() {
            const today = dayjs();
            this.dateNow = today.format ('HH:mm:ss a');
            this.dateDays = today.format ('dddd');
        }
    },
}
</script>

<style scoped lang="scss">
@import '@/styles/variables';
.time {
    width: 100vw;
    background-color:$backgroung-header;
    font-weight: $font-weight-third;
    .header {
        justify-content: center;
        padding: 5px;
        .text {
            padding-right: 15px;
            color: $primary-color-text;
            span {
                text-transform: uppercase;
            }
        }
        i {
            padding-right: 15px;
        }
        .clock {
            padding-right: 30px;
        }
        .geticket {
            padding: 5px 40px;
            background-color: $color-btn;
            color: $color-white;
            transition: transform .4s;
            border: 1px solid transparent;
            &:hover {
                transform: scale(0.9);
                box-shadow: 0 0 0 2px $color-btn;;
                border: 1px solid white;
            } 
        }
    }
}
</style>