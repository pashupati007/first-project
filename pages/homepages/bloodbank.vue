<template>
  <div>
    <v-row>
      <v-col cols="12" lg="8" class="mr-n5 ml-5">
        <div>
          <HomeBloodbanksInsidevalley />
        </div>
        <div>
          <HomeBloodbanksOutsidevalley />
        </div>
      </v-col>

      <v-col cols="12" lg="4">
        <div>
          <HomeBloodbanksBloodbanksearch />
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
