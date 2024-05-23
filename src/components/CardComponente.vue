<template>
    
    <div class="col">
      <div class="card">
        <div class="card-img-wrapper d-flex justify-content-center align-items-center">
            <img :src="card.url" class="card-img m-2" alt="...">

        </div>
          <div class="card-body d-flex justify-content-between">
            <div class="div">
                <h5 class="card-title">{{ card.name }}</h5>
              <p class="card-description fs-6">{{ card.Description }}</p>

            </div>
          <div class="mt-5">
              <p class="card-preco">R$ {{ card.price }}</p>
  
          </div>
        </div>
    </div>
  </div>



</template>


<script>

export default {
  name: 'CardComponente',
  components: {

  },
  data() {
    return {

    }
  },
  props: {
    card: {
      type: Object,
    }
  }
}


</script>


<style scoped>

.card {
    width: 300px;
    height: 200px;
}

.card-title{
    color: #D42401
}


.card-body{
    width: 300px;
    height: 100px;
    background-color: #FED8B5;
}

.card-img{
    width: 215px;
    height: 161px;

}

.card-preco {
    font-size: 20px;
    color: #D42401;
}

span {
    font-size: 40px;
}

</style>