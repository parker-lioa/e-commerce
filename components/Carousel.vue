<template>
    <v-carousel hide-delimiter cycle>
        <v-carousel-item v-for="(slide, i ) in slides" :key="i">
            <v-sheet :color="colors[i]" height="100%">
                <v-row
                    class="fill-height"
                    align="center"
                    justify="center"
                >
                    <div class="text-h2">
                        {{ slide }} Slide
                    </div>
                </v-row>
            </v-sheet>
        </v-carousel-item>
    </v-carousel>
</template>

<script>
export default {
    data(){
        return{
            colors: [
                'indigo',
                'warning',
                'pink darken-2',
                'red lighten-1',
                'deep-purple accent-4',
            ],
            slides:[
                'First',
                'Second',
                'Fourth',
                'Fifth',
            ]
        }
    }
}
</script>