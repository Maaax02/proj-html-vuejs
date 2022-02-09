<template>
    <div class="container">
        <div class="text">
            <p>Joing Over <span>500,000 Students</span> Enjoying Avada Education now</p>
            <p class="gray">Become Part of Avada University  to further your Career.</p>
        </div>
        <div class="label">
            <input type="text" placeholder="Name">
            <input type="text" placeholder="Email">
            <input type="text" placeholder="Telephone">
            <button>APPLY NOW</button>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    .container{
        height: 250px;
        background-color: #272A39;
        text-align: center;
        .text{
            padding-top: 70px;
            padding-bottom: 40px;
            p{
                font-size: 20px;
                color: #fff;
            }
    
            span{
                color: #ffab0b;
            }
    
            .gray{
                color: #94979f;
                font-size: 16px;
            }
        }

        .label{

            input{
                background-color: #667287;
                border: none;
                margin: 0 8px;
                padding: 4px 6px;
                color: #fff;
            }

            button{
                background-color: #ffab0b;
                color: #fff;
                padding: 4px 40px;
                border: none;
            }
        }

    }
</style>