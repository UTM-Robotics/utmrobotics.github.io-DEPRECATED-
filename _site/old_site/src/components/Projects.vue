<template>
  <div>
    <v-carousel
      v-model="model"
      :show-arrows="showArrows"
      :hide-delimiters="hideDelimiters"
      :cycle="cycle"
    >
      <v-carousel-item>
        <v-card
          color="blue"
          height="100%"
          tile
        >
            <v-container fluid>
                <v-row
                    align="center"
                    justify="center"
                >
                    <div class="display-3">Garbage Collector</div>
                    <hr/>
                </v-row>
                <v-row
                    align="center"
                    justify="center"
                >
                    <div>Build a robot that drives around campus, detects and picks up garbage</div>
                </v-row>
                <v-row
                    align="center"
                    justify="center"
                >
                    <div>
                        <v-img 
                            contain 
                            max-height="300"
                            src='@/assets/car.jpg'
                        >
                        </v-img>
                    </div>
                </v-row>
          </v-container>
        </v-card>
      </v-carousel-item>
      <v-carousel-item>
        <v-card
          color="pink"
          height="100%"
          tile
        >
            <v-container fluid>
                <v-row
                    align="center"
                    justify="center"
                >
                    <div class="display-3">Self-Balancing Inverted Pendulum</div>
                    <hr/>
                </v-row>
                <v-row
                    align="center"
                    justify="center"
                >
                    <div>Balance a pendulum vertically on a motor driven wagon.</div>
                </v-row>
                <v-row
                    align="center"
                    justify="center"
                >
                    <iframe 
                        width="560" 
                        height="315" src="https://www.youtube.com/embed/cyN-CRNrb3E" 
                        frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
                        allowfullscreen
                    ></iframe>
                </v-row>
          </v-container>
        </v-card>
      </v-carousel-item>
    </v-carousel>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        items: [
            {
                name: 'Garbage Collector',
                description: 'Build a robot that drives around campus, detects and picks up garbage',
                color: 'primary'
            },
            {
                name: 'Self-Balancing Inverted Pendulum Balancer',
                description: 'See https://www.youtube.com/watch?v=cyN-CRNrb3E',
                color: 'secondary'
            }
        ],
        model: 0,
        showArrows: true,
        hideDelimiters: false,
        cycle: false,
      }
    },
  }
</script>