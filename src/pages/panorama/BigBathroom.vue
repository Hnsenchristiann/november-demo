<template>
    <marzipano 
        sceneUrl="/assets/scenes/BigBathroom_BLANK.jpg"
        :arrows="arrows"
    />
    <!-- <div class="container">
        <div id="viewer" ref="view" class="h-screen-custom w-screen" @click="getCoords">
        </div>
        <div ref="arrowOne" class="arrow-container">
            <router-link to="/panorama/bigroom">
                <div class="text-white">Room view</div>
                <svg xmlns="http://www.w3.org/2000/svg" class="arrow" fill="white" viewBox="0 0 24 24" stroke="black">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 11l3-3m0 0l3 3m-3-3v8m0-13a9 9 0 110 18 9 9 0 010-18z" />
                </svg>
            </router-link>
        </div>
    </div> -->
</template>

<script>
import Marzipano from './components/Marzipano.vue'
export default {
    components: {
        Marzipano
    },
    // beforeDestroy(){
    //     document.body.style.overflow = "visible";
    //     this.marzObj.viewer.destroyAllScenes();
    // },
    // mounted(){
    //     const elem = this.$refs.view
    //     const arrowOne = this.$refs.arrowOne
    //     this.marzObj = createMarzipano(elem, '/assets/scenes/BigBathroom_BLANK.jpg')
    //     this.hotSpots.arrowOne = this.marzObj.scene.hotspotContainer().createHotspot(arrowOne, this.coords.arrowOne)
    //     document.body.style.overflow = "hidden";

    //     document.querySelector('#viewer div').style.height = '100vh'
    //     document.querySelector('#viewer canvas').style.height = '100vh'
    // },
    data(){
        return {
            // marzObj: null,
            // hotSpots: {

            // },
            // coords: {
            //     arrowOne: { yaw: 1.0887977785746852, pitch: 0.13635887604145935 }
            // }
            arrows: [
                {
                    name: 'arrowOne',
                    link: '/panorama/bigroom',
                    title: 'Room view',
                    coord: {
                        yaw: 1.0887977785746852, pitch: 0.13635887604145935
                    }
                },
            ],
        }
    },
    // methods: {
    //     getCoords(e){
    //         console.log(this.marzObj.view.screenToCoordinates({x: e.clientX, y: e.clientY}))
    //     },
    //     updateLocation(){
    //         this.hotSpots.arrowOne.setPosition(this.coords.arrowOne)
    //     }
    // }
}
</script>

<style>
    .arrow-container{
        width: 70px;
        height: 70px;
        margin-left: -35px;
        margin-top: -70px;
        text-align: center;
        width: 100px;
        text-shadow: rgb(0 0 0) -1px -1px 0px, rgb(0 0 0) 1px -1px 0px, rgb(0 0 0) -1px 1px 0px, rgb(0 0 0) 1px 1px 0px;
    }
    .arrow{
        width: 60px;
        height: 60px;
        margin: auto;
    }
</style>