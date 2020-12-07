<template>
    <div id="brend">
        <div class="brend">
            <h2>Brendlar</h2>
        <hr class="line">
        <p>Hamma Brendlar <i class="fas fa-angle-double-right"></i></p>
        <div class="next">
            <button @click="back"> <i class="fas fa-chevron-left"></i> </button>
            <button @click="font"> <i class="fas fa-chevron-right"></i> </button>
        </div>
        </div>
        <div class="icons">
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
        </div>
    </div>
</template>



<style scoped>
#brend{
    width: 100%;
    padding: 20px 30px;
    overflow: hidden;
}
.brend{
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
    background-color: none;
    background: none;
    border: .5px solid gray;
}
.next button:hover {
    background: gold;
    border: none;
}
.icons{
    position: relative;
    display: inline-flex;
    transition: .5s;
}
.icons div{
    margin: 0 20px;
    width: 10vh;
    height: 10vh;
    background:url("../assets/logo.png");
    background-size: cover;
    transition: .5s;
}

</style>