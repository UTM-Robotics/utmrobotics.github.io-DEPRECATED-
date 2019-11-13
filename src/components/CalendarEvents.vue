<script>
  export default {
    data: () => ({
      events: [
        {
          name: 'Tabling',
          start: '2019-11-14 14:00',
          end: '2019-11-14 16:00',
          color: 'indigo',
          info: '2019-11-14, 2-4pm, Location TBD',
          description: 
            "Meet some of the Robotics Club execs and take a look at some of the projects we're working on!"
        },
        {
          name: 'Weekly Meeting',
          start: '2019-11-15 16:00',
          end: '2019-11-15 17:00',
          color: 'blue',
          info: "2019-11-15, 4-5pm, DH3003",
          description:
            "Join us as we discuss the future of the club and plan upcoming events and projects. Everyone is welcome"
        },
        {
          name: 'Arduino Workshop 2',
          start: '2019-11-19 16:00',
          end: '2019-11-19 18:00',
          color: 'deep-orange',
          info: '2019-11-19, 4-6pm, DH 2020',
          description: 
            "Introduction to arduinos- covering the basics of inputs and outputs, electricity, applications, and most importantly safety"
        },
        {
          name: '3D Printing Workshop',
          start: '2019-11-22 15:00',
          end: '2019-11-22 14:00',
          color: 'pink',
          info: "2019-11-22, 3-4pm, DH3003",
          description:
            "Setting up a 3D printer and configuring settings for high quality prints"
        }
      ],
    }),
  }
</script>