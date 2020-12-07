<template>
    <div id="card">
        <div class="cards">
            <h2>Xitlar</h2>
        <hr class="line">
        <p>Hamma Xitlar >></p>
        <div class="next">
            <button> <i class="fas fa-chevron-left"></i> </button>
            <button> <i class="fas fa-chevron-right"></i> </button>
        </div>
        </div>
        <div class="item">
            <div v-for="item in items" :key="item">
            <Card :name="item.name" :prize="item.prize"/>
        </div>
        
        </div>
    </div>
</template>

<script>
import Card from "./Card"
export default {
    components:{
        Card
    },
    data(){
        return{
            items:[
                {
                    name:"Telvezor Samsung 54",
                    prize:"1 299 900"
                },
                {
                    name:"Mac Book pro 13",
                    prize:"15 299 900"
                },
                {
                    name:"Telvezor Samsung 54",
                    prize:"1 299 900"
                },
                {
                    name:"Mac Book pro 13",
                    prize:"15 299 900"
                },
                {
                    name:"Telvezor Samsung 54",
                    prize:"1 299 900"
                },
                {
                    name:"Mac Book pro 13",
                    prize:"15 299 900"
                }
            ]
        }
    },
}
</script>

<style scoped>
#card{
    width: 100%;
    padding: 20px 30px;
}
.cards{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.line{
    border-top: 1px solid gray;
    width: 75%;
    padding: 0 20px;
}
.next button {
    width: 30px;
    height: 30px;
    margin-left: 10px;
    background: none;
    border: .5px solid gray;
}
.next button:hover {
    background: gold;
    border: none;
}
.item{
    position: relative;
    display: flex;
    width: 100%;
    overflow: hidden;
}
</style>