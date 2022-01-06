<template>
  <div>
    <v-container>
      <v-row>
        <v-col>
          <p class=".donate text-lg-h3 text-md-h4  mt-5 font-weight-bold">
            DONATE BLOOD,<br />
            Save a Life!
          </p>
        </v-col>
      </v-row>

      <v-row>
        <v-col>
          <p class=".donate text-lg-h5 text-md-h6 font-weight-regular mt-n5 mb-10">
            Your donation will go to save countless lives and so is appreciated,
            time and <br />
            time again. <br />
            I hope you know how much your blood is a gift to another's life
          </p>
        </v-col>
      </v-row>
   
      <v-row>
        <v-col>
          <v-btn class="mt-16 pt-5 pb-5 font-weight-bold">
            DONATE NOW 
            <v-img class="mb-1 " :src="require('~/assets/img/dropbtn.png')" width="70" height="70"></v-img>
          </v-btn>
        </v-col>
      </v-row>
    </v-container>

    
  </div>
</template>

<style>
  .donate{
    font-family: Poppins;
  }
</style>