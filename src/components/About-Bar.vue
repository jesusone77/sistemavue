<template>
  <v-container>
    <v-row class="text-left">
      <v-col>
        <h1 class="display-2 font-weight-bold mb-3">
          {{ title }}
        </h1>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  props:['title'],
  setup() {
    return {
      
    }
  },

}
</script>
