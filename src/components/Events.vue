<template>
  <v-tabs
    fixed-tabs
  >
    <v-tab>
      Upcoming
    </v-tab>
    <v-tab>
      Previous
    </v-tab>
    <v-tab>
      Calendar
    </v-tab>

    <v-tab-item>
        <Upcoming/>
    </v-tab-item>
    <v-tab-item>
    
    </v-tab-item>
    <v-tab-item>
    
    </v-tab-item>
  </v-tabs>
</template>

<script>
import Upcoming from '@/components/Upcoming'
export default {
  name: 'Events',
  components: {
    Upcoming
  }
}
</script>