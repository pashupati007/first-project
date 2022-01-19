<template>
  <div>
    <div class="pa-10">
      <v-card
        :height="height"
        :width="width"
        class="back"
      >
    <LoginFixedlogincomponentsAppbar />
        <LoginLoginhome />
   </v-card>
    </div>

    <div>
      <LoginAbout />
    </div>

    <div>
      <LoginWhy />
    </div>

    <div>
      <LoginBlogs />
    </div>

    <div>
      <LoginContact />
    </div>
  </div>
</template>

<script>
export default {
  layout: "loginlayouts/loginlayouts",
  data() {
    return {
      height: 0,
      width: 0,
    };
  },
  mounted() {
    this.height = window.innerHeight - 100;
    this.width = window.innerWidth;
  },
  // created(){

  // },
  // watch:{
  //     email(newValue,oldValue){
  //       if(newValue.length>10){
  //         this.msg='Number should not be greater than 10'
  //       }
  //     }
  // },
  // methods:{

  // }
};
</script>

<style>
.back {
  background-size: 40% 50%;
  background-image: url("~/assets/img/loginimg/hand.png") !important;
  background-image: no-repeat;
  background-position: center bottom;
  box-shadow: 0 25px 15px rgba(0, 0, 0, 0.16) !important;
}
</style>
