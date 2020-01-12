<template>
    <v-app>
        
        <v-content>
            <ImgBar/>
            <Warning/>
            <!-- <Grid/> -->
            <Main/>
        </v-content>
    </v-app>
</template>

<script>
    import ImgBar from './components/ImgBar'
    // import Grid from './components/Grid'
    import Main from './components/Main'
    import Warning from './components/Warning'

    export default {
        name: 'App',
        components: {
            ImgBar,
            // Grid,
            Main,
            Warning
        },
        data: () => ({
            //
        }),
    };
</script>
