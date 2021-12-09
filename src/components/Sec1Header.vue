<template>
    <section class="time">
        <div class="container d-flex header align-items-baseline">
            <div class="text"> 
                <p>Starts <span>tomorrow!</span> Our biggest event of the year...</p> 
            </div>
            <div class="d-flex align-items-baseline">
                <i class="far fa-clock"></i>
                <p class="clock">00 : 00 : 00 : 00</p>
                <button type="button" class="btn geticket">Get ticket</button>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Sec1Header'
}
</script>

<style scoped lang="scss">
.time {
    width: 100vw;
    background-color:#f5f5f5;
    font-weight: 200;
    .header {
        justify-content: center;
        padding: 5px;
        .text {
            padding-right: 15px;
            color: #777777;
            span {
                text-transform: uppercase;
            }
        }
        i {
            padding-right: 15px;
        }
        .clock {
            padding-right: 50px;
        }
        .geticket {
            padding: 5px 40px;
            background-color: #ef6f31;
            color: white;
        }
    }
}
</style>