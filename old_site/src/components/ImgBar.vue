<template>
<v-card>
    <v-toolbar
        app 
        color="#fcb69f"
        dark 
        src="@/assets/utm-robotics-header.jpg" 
    >
        <!-- <v-spacer></v-spacer> -->
        <!-- <v-avatar size="48" color="white" left>
            <img src="@/assets/Artboard1.png" alt="logo">
        </v-avatar> -->
        <v-toolbar-title class="headline text-uppercase">
            <h3>UTM Robotics Club</h3>
        </v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn icon href="https://twitter.com/utmrobotics" target="_blank">
            <v-icon>mdi-twitter</v-icon>
        </v-btn>
        <v-btn icon href="https://www.facebook.com/utmrobotics" target="_blank">
            <v-icon>mdi-facebook</v-icon>
        </v-btn>
        <v-btn icon href="https://www.instagram.com/utm_robotics/" target="_blank">
            <v-icon>mdi-instagram</v-icon>
        </v-btn>
        <v-btn 
            icon 
            href="https://join.slack.com/t/utmrobotics/shared_invite/enQtNzY5OTM0NzA0NTc3LWZkODEwZmJlMDljOGVlNWFhODI0OGVjMzdkOGQ4YmIwODA2YzUxNDM5NGE2NDI4YThhMDkyOTc2OTAwZjJlMjM" 
            target="_blank"
        >
            <v-icon>mdi-slack</v-icon>
        </v-btn>
    </v-toolbar>
</v-card>
</template>