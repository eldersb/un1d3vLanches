<template>
 
    <div class="container">
     <div class="row">
   
      
       <div class="div">
           <h3 class=" sub-titulo text-center mt-5">
             Vai ficar só na vontade? Escolha agora mesmo o seu lanche <br>
             e gere seu <span>Código promocional</span> ;)
           </h3>
         </div>
   
         <section class="mt-5">

          <article class="row row-cols-1 row-cols-md-3 g-5 r">

            <template v-for="card in allCards" :key="card.id">
  
              <CardComponente :card="card" class="mb-5" />
            </template>
          </article>
   

         </section>
             
   
     </div>
    </div>
   
   </template>
   
   <script>
   import CardComponente from '../components/CardComponente.vue';
   import axios from 'axios';

   
   
   
   export default {
     name: 'HomeView',
     components: {
       CardComponente
     },
     data(){
       return {
         allCards: []
   
       }
     },
     created() {
    this.fetchData();
    },
    methods: {
      async fetchData(){
        try {
          const responseCards = await axios.get('http://localhost:3000/devLanches')
          this.allCards = responseCards.data;
        }

      catch(error){
        console.error('Erro ao buscar dados:', error);

      }
    } 
  }
 }
   </script>
   
   <style>
   
   body {
    background-color:#F5EBDC ;
   }

   span {
     color: #D42401;
   }
   
   .sub-titulo {
     font-size: 20px;
   }

   .custom-gutter > * {
  margin-bottom: 50px; /* Ajuste o valor conforme necessário */
}
   
   
   
   </style>
   