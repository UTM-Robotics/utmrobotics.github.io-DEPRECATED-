<template>
    <v-container>
        <v-row-dense>
            <v-col
                v-for="(item, i) in items"
                :key="i"
                cols="12"
            >
                <v-card :color="item.color" dark>
                  <v-card-title class="headline" v-text="item.name"></v-card-title>
                  <v-card-subtitle v-text="item.info"></v-card-subtitle>
                  <v-card-text>
                    {{ item.description }}
                  </v-card-text>
                </v-card>
            </v-col>
        </v-row-dense>
    </v-container>
</template>


<script>
  import CalendarEvents from '@/components/CalendarEvents';

  export default {
    data: () => ({
      items: CalendarEvents.data().events
    }),
  }
</script>