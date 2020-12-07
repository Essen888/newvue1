
<template>
  <div id="app">
   
   <button class="button" @click="toggleElement">Узнать больше/ Cвернуть</button>
    <div class="wrap">
   <div class="element" v-if="isElvisible">Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis, adipisci! Necessitatibus, laboriosam quas? Debitis harum odio aperiam, maiores qui fuga ea dolorum sapiente corrupti sit distinctio quasi natus, asperiores quia.
     Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus aperiam sequi ratione ipsum voluptates earum alias! Mollitia, aspernatur incidunt! Quis eum doloremque non, earum eveniet expedita tempora autem et nemo!
   </div>
  </div>
  </div>
</template>

<script>
export default {
  name: "app",
  data:() => {
    return{
 isElvisible:true
    }
  },
methods: {
  toggleElement(){
    this.isElvisible= !this.isElvisible
  }
}
};
</script>

<style>

.button{
    margin-top:40px;
    min-width: 220px; 
    min-height: 30px;
    background-color:  #ff510c;
    color:aliceblue;

    }
.element{
  border: #ff510c dashed 5px;
  max-width: 400px;
  margin: 10px;
  padding: 5px;
  
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #717537;
  margin-top: 60px;
}
.wrap{
  display: flex;
  justify-content: center;
}
</style>
