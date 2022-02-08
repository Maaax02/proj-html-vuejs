<template>
    <div class="container">
        <div class="image">
            <img src="../../public/img/university_logo.png" alt="">
        </div>
            
            <div class="right">
                <ul>
                    <li v-for="(item, i) in nav" :key="i">
                        {{item}}
                    </li>
                </ul>
            </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            nav : [
                'HOME',
                'ABOUT',
                'COURSES',
                'EVENTS',
                'FACILITIES',
                'NEWS',
                'ADMISSIONS'
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.container{
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 130px;

    ul{
        list-style: none;
        display: flex;

        li{
            margin-left: 40px;
        }
    }
}
</style>