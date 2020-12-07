<template>
    
        <ul class="card" >
            <li class="Item" >
                <div class="img"></div>
                <hr>
                <p class="itemName">{{name}}</p>
                <hr class="prizeLine">
                <p class="itemPrize">{{prize}} sum</p>
                <div class="add">
                    <button @click="minus" v-if="count !== 0">-</button>
                    <p v-if="count !== 0">{{count}}</p>
                    <button @click="plus" class="plus">+</button>
                </div>
            </li>
        </ul>
    
</template>

<script>
export default {
    
    props:["name", "prize"],
    data(){
        return{
            count:0
        }
    },
    methods:{
        plus(){
            this.count++
        },
        minus(){
            this.count--;
            if(this.count === -1){
                this.count = 0
            }

        }
    }
}
</script>

<style scoped>

.card{
    padding: 20px 0;
    display: flex;
    overflow: hidden;
}
.Item{
    width: 30vh;
    height: 50vh;
    border: 1px solid lightgray;
    background: white;
    transition: .5s;
}
.Item:hover{
    transform: scale(1.05);
}
.itemName{
    padding: 15px 10px;
    font-size: 16px;
    font-weight: bolder;
}
.itemPrize{
    padding: 10px 10px;
    font-size: 16px;
}
.img{
    width: 100%;
    height: 30vh;
    margin: auto;
    background: url("../assets/mac.jpg");
    background-position: center;
    background-size: cover;
}
.prizeLine{
    background: gold;
    border: none;
    width: 20%;
    height: 3px;
    margin: 0 10px;
}
.add{
    display: flex;
    align-items: center;
    justify-content: flex-end;
    padding: 0 20px;
}
.add button {
    width: 30px;
    height: 30px;
    border: none;
    border-radius: 50%;    
}
.add p{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 10vh;
    border: 1px solid;
    margin: 0 20px;
    background: none ;
    border-radius: 20px;
    height: 30px;
}
.plus{
    background: gold;
}
</style>