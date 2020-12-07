<template>
    <nav>
        <div class="logo">
            <h1>LOGO</h1>
        </div>
        <div class="bar">
            <input type="text" placeholder="Qidirish...">
            <select name="select" id="kotegorya">
                <option value="#">Barcha kategoriyalar</option>
            </select>
            <button><i class="fas fa-search"></i></button>
            <i class="fas fa-user"></i>
            <i class="fas fa-shopping-cart"></i>
        </div>
    </nav>
</template>




<style scoped>
nav{
    width: 100%;
    height: 10vh;
    background: #fafafa;
    padding: 0 30px;
    display: grid;
    grid-template-columns: 20% 80%;
    align-items: center;
    justify-content: space-between;
}
.bar{
    display: flex;
    justify-content: flex-end;
    align-items: center;
}

.bar input{
    width: 80%;
    padding: 0 20px;
    height: 5vh;
}
.bar select{
    width: 26vh;
    padding: 0 20px;
    height: 5vh;
}
.bar input select {
    border: 1px solid rgba(128, 128, 128, 0.6);
}
.bar button{
    width: 5vh;
    height: 5vh;
    background: gold;
    border: none;
}
.bar .fa-user{
    padding: 0 20px;
}
@media only screen and (max-width:600px) {
  .bar input, select{
      display: none;
  }
}
</style>