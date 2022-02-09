<template>
    <div class="container">
        <div v-for="(item, i) in here" :key="i" :class="item.class">
            <h2>{{item.title}}</h2>
            <div class="line"></div>
            <span>{{item.text}}</span>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            here : [
                {
                    class:'left',
                    title: 'COURSES',
                    text : 'View More'
                },
                {
                    class: 'middle',
                    title : 'EVENTS',
                    text : 'View More'
                },
                {
                    class : 'right',
                    title: 'LATEST NEWS',
                    text : 'View More'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .container{
        display: flex;
        color: #fff;
        
        .left{
            background-image: url("../../public/img/home_courses_section_bg.jpg") ;
            background-size: cover;
            height: 800px;
            width: calc(100% / 3);
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }

        .middle{
            background-image: url("../../public/img/home_events_section_bg.jpg") ;
            background-size: cover;
            height: 800px;
            width: calc(100% / 3);
             display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }

        .right{
            background-image: url("../../public/img/home_latest_news_section_bg.jpg") ;
            background-size: cover;
            height: 800px;
            width: calc(100% / 3);
             display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }

        .line{
            margin: 20px 0;
            width: 45px;
            border-bottom: 1px solid #FFAB0B;
        }
    }
</style>