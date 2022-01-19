<template>
  <div>
    <v-row>
      <v-col cols="12" lg="9">
        
        <div>
          <HomeBloodfeedsBlooddrop />
        </div>

        <div>
          <HomeBloodfeedsBlooddonors />
        </div>

        <div>
          <HomeBloodfeedsDonateblood />
        </div>

        <div>
          <HomeBloodfeedsDonationcampaign />
        </div>

      </v-col>

      <v-col cols="12" lg="3">

        <div>
          <HomeBloodfeedsDonorsearch />
        </div>

        <div>
          <HomeBloodfeedsNewdonor />
        </div>

      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {

  layout: "homelayouts",
};
</script>
