<template>
    <div class="container">
        <main>
            <div class="left">
                <h1>WORLD CLASS FACILITIES</h1>
                <p>Avada university is devoted to exellence in teaching learning and research, and developing leaders in many disciplineswho make a difference globally</p>
            </div>
            <div class="right">
                <h1>OUR VALUES</h1>
                <div class="our-box" v-for="(item, i) in values" :key="i"><span>+</span> {{item}}</div>
            </div>
        </main>
    </div>
</template>

<script>
export default {
    data(){
        return{
            values : [
                'OUR MISSION',
                'OUR PHILOSOPHY',
                'OUR COMMITMENT',
                'OUR PROMISE',
                'OUR VALUES'
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.container{
    background-color: #E6E6E6;
    height: 600px;
    
    main{
        display: flex;
        width: 1300px;
        margin: 0 auto;

        .left{

        }
    }
    .our-box{
        width: 700px;
        margin: 6px 0;
        padding: 10px 20px;
        color: #ffab0b;
        background-color: #fff;
        font-size: 20px;
        font-weight: bold;

        span{
            font-size: 25px;
            margin-right: 10px;
        }
    }
}
</style>