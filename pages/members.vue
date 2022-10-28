<template>
  <div>
    <Nav />
    <br />
    <h1>メンバー紹介</h1>
    <br />
    <v-container class="grey lightne-5">
      <v-row>
        <v-col>
          <v-img src="/membertop.jpg"></v-img>
        </v-col>
      </v-row>
    </v-container>
    <br /><br />
  </div>
</template>

<script>
  export default {
    data(){
      return{
        user:'test user',
        usedtime:5,
      }
    }
  };
</script>

<style>
.texto{
  font-size: 2rem;
  color:orange;
}
</style>