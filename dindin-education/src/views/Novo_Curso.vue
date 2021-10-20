<template>
  <div class="novo">
    <form id="novo-curso-form" @submit="createCurso">  
    <h1>Novo Curso</h1>
    <div>
      
          <div class="input-container">
              <label for="titulo"></label>
              <input type="text" id="titulo" name="titulo" v-model="titulo" placeholder="Titulo">
          </div>
          <div class="input-container">
              <label for="capa"></label>
              <input type="text" id="capa" name="capa" v-model="capa" placeholder="upload capa">
          </div>
          <div class="input-container">
              <label for="prof"></label>
              <input type="text" id="prof" name="prof" v-model="prof" placeholder="Professor">
          </div>
          <div class="input-container">
              <label for="desc"></label>
              <input type="text" id="desc" name="desc" v-model="desc" placeholder="Descrição">
          </div>
      
  </div>
  <h2> Aula 1 </h2>
  <div>
     
          <div class="input-container">
              <label for="titulo_aula"></label>
              <input type="text" id="titulo_aula" name="titulo_aula" v-model="titulo_aula" placeholder="Titulo da aula">
          </div>
          <div class="input-container">
              <label for="link"></label>
              <input type="text" id="link" name="link" v-model="link" placeholder="Link da aula">
          </div>
          <div class="input-container">
              <label for="desc_aula"></label>
              <input type="text" id="desc_aula" name="desc_aula" v-model="desc_aula" placeholder="Descrição da aula">
          </div>
         
  
  </div>
  <h2> Aula 2 </h2>
  <div>
      
          <div class="input-container">
              <label for="titulo_aula"></label>
              <input type="text" id="titulo_aula" name="titulo_aula" v-model="titulo_aula" placeholder="Titulo da aula">
          </div>
          <div class="input-container">
              <label for="link"></label>
              <input type="text" id="link" name="link" v-model="link" placeholder="Link da aula">
          </div>
          <div class="input-container">
              <label for="desc_aula"></label>
              <input type="text" id="desc_aula" name="desc_aula" v-model="desc_aula" placeholder="Descrição da aula">
          </div>
         
   
  </div>
  <h2> Aula 3 </h2>
  <div>
  
          <div class="input-container">
              <label for="titulo_aula"></label>
              <input type="text" id="titulo_aula" name="titulo_aula" v-model="titulo_aula" placeholder="Titulo da aula">
          </div>
          <div class="input-container">
              <label for="link"></label>
              <input type="text" id="link" name="link" v-model="link" placeholder="Link da aula">
          </div>
          <div class="input-container">
              <label for="desc_aula"></label>
              <input type="text" id="desc_aula" name="desc_aula" v-model="desc_aula" placeholder="Descrição da aula">
          </div>
         
     
  </div>
  <div class="input-container">
      <input type="submit" class="submit-btn" value="Salvar">
  </div>
  </form>   
  </div>
</template>

<script>
export default {

methods:{
    async createCurso(e) {
        e.preventDefault();

        const data = {
            titulo: this.titulo,
            capa: this.capa,
            prof: this.prof,
            desc: this.desc,
            
        }
        
    }
}
}
</script>

<style>
.novo{
  margin: 0 auto;
  padding: 0 auto;
  text-align: center;
  margin-top:150px;
  background: rgb(8, 173, 63);
}
</style>
