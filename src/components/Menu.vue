<template>
    <div id="menu">
        <div class="menu">
            <div class="category">
            <h4>Kategoryalar</h4>
            <i class="fas fa-bars"></i>
        </div>
        <div class="menu-bar">
            <a href="#">Bosh sahifa</a>
            <a href="#">Biz haqimizda</a>
            <a href="#">Chegirmalar</a>
            <a href="#">Biz bilan aloqa</a>
        </div>
        </div>
        <div id="category-menu">
            <div class="category-menu">
                <a href="#" v-for="category in categories" :key="category"> 
                    <i :class="category.icon"></i>
                    <p>{{category.name}}</p>
                </a>
            </div>
            <div class="categories">
               <div class="catigory-select" v-for="select in selected" :key="select">
                   <h3>{{select.name}}</h3>
                   <a href="#" v-for="component in select.comp" :key="component">
                       {{component}}
                   </a>
               </div>
               <div class="show">
                   <div class="blur">
                       <h1>LOGO</h1>
                   </div>
               </div>
            </div>
        </div>
    </div>
</template>


<script>
export default {
    data(){
        return{
            active:"",
            categories:[
                        {icon:"fas fa-utensils", name:"Oziq-ovqat mahsulotlari"},
                        {icon:"fas fa-utensils", name:"Maishiy texnika vositalari "},
                        {icon:"fas fa-utensils", name:"Telfon va aksessuarlar"},
                        {icon:"fas fa-utensils", name:"Maishiy texnika"},
                        {icon:"fas fa-utensils", name:"Oshxona texnikasi"},
                        {icon:"fas fa-utensils", name:"Sport anjomlari"},
                        {icon:"fas fa-utensils", name:"Go'zallik va salomatlik"},
                        {icon:"fas fa-utensils", name:"Avto jxozlar"},
                        {icon:"fas fa-utensils", name:"Barcha ofis, uy va bog' uchun"},
                        {icon:"fas fa-utensils", name:"Bolalar uchun o'yinchoqlar"},
                    ],
            selected:[
                {
                    name: "Sabzavot va mevalar",
                    comp:[
                        "Hammasi",
                        "Sabzavodlar",
                        "Mevalar",
                        "Ko'katlar",
                        "Quritilgan mevalar"
                    ]
                },
                 {
                    name: "Sabzavot va mevalar",
                    comp:[
                        "Hammasi",
                        "Sabzavodlar",
                        "Mevalar",
                        "Ko'katlar",
                        "Quritilgan mevalar"
                    ]
                },
                 {
                    name: "Sabzavot va mevalar",
                    comp:[
                        "Hammasi",
                        "Sabzavodlar",
                        "Mevalar",
                        "Ko'katlar",
                        "Quritilgan mevalar"
                    ]
                }
                ,
                 {
                    name: "Sabzavot va mevalar",
                    comp:[
                        "Hammasi",
                        "Sabzavodlar",
                        "Mevalar",
                        "Ko'katlar",
                        "Quritilgan mevalar"
                    ]
                },
                 {
                    name: "Sabzavot va mevalar",
                    comp:[
                        "Hammasi",
                        "Sabzavodlar",
                        "Mevalar",
                        "Ko'katlar",
                        "Quritilgan mevalar"
                    ]
                }
                
            ]
        }
    },
    
}
</script>


<style scoped>

.menu{
    width: 100%;
    padding: 0 30px;
    border-top: 1px solid rgb(182, 182, 182);
    border-bottom: 1px solid rgb(182, 182, 182);
    background: #fafafa;
    display: grid;
    grid-template-columns: 20% 80%;
}
.category{
    border: none;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0 20px;
    height: 6vh;
    background:  #040397;
    color: white;
}
.menu-bar{
    height: 6vh;
    display: flex;
    align-items: center;
    justify-content: flex-end;
}
.menu a{
    padding: 0 20px;
    color: black;
}
#category-menu{
    display: grid;
    grid-template-columns: 20% 80%;
    padding: 0 30px;
}
.category-menu{
    display: grid;
    text-align: start;
}
.category-menu a:hover{
    background: gold;
    color: white;
}
.category-menu a{
    width: 100%;
    height: 7vh;
    border: 1px solid lightgray;
    display: flex;
    align-items: center;
    color: black;
    padding: 0 40px;
    justify-content: flex-start;
}

.category-menu a i{
    padding: 0 5px;
}
.categories{
    padding: 20px;
    height: 70vh;
    box-shadow: 0 0 10px rgb(199, 199, 199);
    display: grid;
    grid-template-columns: 33% 33% 33%;
    
}
.catigory-select a{
    display: grid;
    padding: 10px 20px;
}
.show{
    display: flex;
    align-items: center;
    justify-content: center;
    background: url("../assets/f.jpg");
    background-size: cover;
}
.blur{
    display: flex;
    align-items: center;
    justify-content: center;
    backdrop-filter: blur(2px);
    background-color: rgba(255, 255, 255, 0.7);
    width: 80%;
    height: 80%;
}
@media only screen and (max-width:600px) {
    .menu{
        grid-template-columns: 100%;
    }
    .menu-bar{
        display: none;
    }
    #category-menu{
        grid-template-columns: 100%;
    }
    .categories{
        display: none;
    }
}
</style>