<template>
  <v-card rounded="lg" class="pa-md-10 pa-5 text-center" color="primary" dark>
    <h2 class="text-md-h3">Newsletter</h2>
    <p class="text-md-h6 mt-5">Subscribe to receive</p>
    <br/>

    <v-sheet color="transparent" class="mx-auto" max-width="400">
      <!-- <v-text-field label="Email" type="email" outlined v-model="email"> </v-text-field>-->
      <v-btn outlined min-height="50" block href="https://forms.gle/7nzyXjGH5H61j3hG6" target="_blank" rel="noopener noreferrer">フォームの入力</v-btn>
    </v-sheet>
  </v-card>
</template>
  
  <script>
  export default {
    data(){
      return{
        email: null
      }
    },
  };
  </script>
  
  <style></style>