<template>
    <header class="nav">

        <div class="container">

            <nav class="d-flex justify-content-between align-items-center mt-3 mb-3 gap-2">
              <div class="d-flex align-items-center">

               <a href="/"><img  src="../assets/logo-hamburguer.png" alt="..."></a> 
                <div class="ms-4">
                  <h1 class="mb-0">UN1D3V Lanches</h1>
                  <p class="mb-0">Código e Lanches</p>
                </div>
              </div>
                <a href="/about"  class="btn ml-5"><img class="icone-carrinho" src="../assets/carrinho.png" alt="icone carinho"></a> 
              </nav>
        </div>

    </header>
    
</template>


<style scoped>

header {
  border-bottom: 5px solid #FED8B5;
}

.nav {
  background-color: #F5EBDC;
}

h1 {
  color: #D42401;
  font-size: 28px
}

.icone-carrinho {
  width: 32px;
  height: 32px;
}

</style>