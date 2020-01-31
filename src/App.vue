<script>

export default {
  name: 'App',

  data: () => ({
    //
  })
}
</script>

<template>
  <v-app>
    <div class="container">
      <div :style="{'grid-area':'button' + item}" v-for="item in 9" :key="item">
        <v-btn class="ma-2" outlined large fab color="indigo" >
        {{item}}
      </v-btn>
      </div>
    </div>
  </v-app>
</template>

<style scoped>
  .container {
    display: grid;
    grid-template-columns: repeat(4, 75px);
    grid-template-areas: "button7 button8 button9 ." "button4 button5 button6 ." "button1 button2 button3 .";
  }
</style>
