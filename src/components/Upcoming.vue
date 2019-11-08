<template>
    <v-container>
        <v-row-dense>
            <v-col
                v-for="(item, i) in items"
                :key="i"
                cols="12"
            >
                <v-card :color="item.color" dark>
                  <v-card-title class="headline" v-text="item.title"></v-card-title>
                  <v-card-subtitle v-text="item.date"></v-card-subtitle>
                  <v-card-text>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit, doloremque necessitatibus pariatur iste repellat quaerat rem, ab laudantium delectus eius facere ex dolore vitae odit animi numquam, aperiam commodi nulla?
                  </v-card-text>
                </v-card>
            </v-col>
        </v-row-dense>
    </v-container>
</template>


<script>
  export default {
    data: () => ({
      items: [
        {
          color: '#1F7087',
          src: '',
          title: 'Arduino Workshop',
          date: 'Tues, Oct 12, 7:00PM, DH2020',
        },
        {
          color: '#952175',
          src: '',
          title: 'Arduino Workshop 2',
          date: 'Wed, Nov 15, 4:00PM, IB250',
        },
      ],
    }),
  }
</script>