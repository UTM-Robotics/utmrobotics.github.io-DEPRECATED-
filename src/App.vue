<template>
    <v-app>
        
        <v-content>
            <ImgBar/>
            <Grid/>
        </v-content>
    </v-app>
</template>

<script>
    import ImgBar from './components/ImgBar'
    import Grid from './components/Grid'

    export default {
        name: 'App',
        components: {
            ImgBar,
            Grid
        },
        data: () => ({
            //
        }),
    };
</script>
