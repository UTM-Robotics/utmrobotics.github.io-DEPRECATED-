<template>
  <v-container class="grey lighten-5">
    <v-row>
      <v-col
        cols="8"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          <Events/>
        </v-card>
      </v-col>
      <v-col
        cols="4"
      >
        <v-card
          class="pa-2"
          outlined
          tile
        >
          Second of two columns
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Events from '@/components/Events'

export default {
  name: 'Grid',
  components: {
    Events
  },
  data: () => ({
    //
  }),
  
};
</script>