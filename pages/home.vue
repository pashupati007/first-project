<template>
  <div>

      <v-row>
        <v-col cols="12" lg="8"> 
          <div>
            <UserPost />
          </div>
        </v-col>

        <v-col cols="12" lg="3">
          <div>
            <UserDonarsearch />
          </div>
          <div>
            <UserNewdonor />
          </div>
        </v-col>
      </v-row>

  </div>
</template>
<script>
export default {
  layout: "user",
};
</script>
