<template>
    <div class="bg-blurgh pb-16">
        <div style="color: white; text-align: center; font-size: 90px;">DSI</div>

        <div class="px-4">
            <hr class="my-2" />
        </div>

        <div class="mt-10">
            <div>
                <router-link :to="'/bells-society/'" class="link-type">
                    <img :src="bellsSocietyLogo" style=" width: 100px; display: block; margin-left: auto; margin-right: auto;" />
                    <p class="company-title">Bells <strong>Society</strong></p>
                </router-link>
            </div>

            <div class="mt-12">
                <router-link :to="'/senormal/'" class="link-type">
                    <img :src="senormalLogo" style=" width: 100px; display: block; margin-left: auto; margin-right: auto;" />
                    <p class="company-title"><strong>Senormal</strong></p>
                </router-link>
            </div>

            <div class="mt-12">
                <router-link :to="'/nirmana-kinetik/'" class="link-type">
                    <img :src="nirmanaLogo" style=" width: 350px; display: block; margin-left: auto; margin-right: auto;" />
                </router-link>
            </div>

            <div class="mt-12">
                <router-link :to="'/matahari/'" class="link-type">
                    <img :src="matahariLogo" style=" width: 100px; display: block; margin-left: auto; margin-right: auto;" />
                    <img :src="matahariTextLogo" style=" width: 270px; display: block; margin-left: auto; margin-right: auto;" />
                </router-link>
            </div>

            <div class="mt-12">
                <router-link :to="'/bluesville/'" class="link-type">
                    <img :src="bluesvilleLogo" style=" width: 200px; display: block; margin-left: auto; margin-right: auto;" />
                    <p class="company-title">bluesville</p>
                </router-link>
            </div>

            <div class="mt-12">
                <router-link :to="'/biomagg/'" class="link-type">
                    <img :src="biomaggLogo" style=" width: 200px; display: block; margin-left: auto; margin-right: auto;" />
                    <p class="company-title">Biomagg</p>
                </router-link>
            </div>

            <div class="mt-12">
                <router-link :to="'/bobobox/'" class="link-type">
                    <img :src="boboboxLogo" style=" width: 180px; display: block; margin-left: auto; margin-right: auto;" />
                </router-link>
            </div>

            <div class="mt-12">
                <router-link :to="'/fabelio/'" class="link-type">
                    <img :src="fabelioLogo" style=" width: 105px; display: block; margin-left: auto; margin-right: auto;" />
                    <p style="text-align: center; color: white; font-size: 45px;">Fabelio</p>
                </router-link>
            </div>

            <div class="mt-12">
                <router-link :to="'/visi8/'" class="link-type">
                    <img :src="visiLogo" style=" width: 180px; display: block; margin-left: auto; margin-right: auto;" />
                </router-link>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'landing',
    data(){
        return {
            bellsSocietyLogo: require('../assets/images/bells_society/Picture1.png'),
            senormalLogo: require('../assets/images/senormal/logo.png'),
            matahariLogo: require('../assets/images/matahari/logo.png'),
            matahariTextLogo: require('../assets/images/matahari/text_logo.png'),
            bluesvilleLogo: require('../assets/images/bluesville/logo.png'),
            biomaggLogo: require('../assets/images/biomagg/logo.png'),
            boboboxLogo: require('../assets/images/bobobox/boboboxLogo.png'),
            fabelioLogo: require('../assets/images/fabelio/logo.png'),
            nirmanaLogo: require('../assets/images/nirmana_kinetik/logo-white.png'),
            visiLogo: require('../assets/images/visi8/Logo.png'),
        }
    },
    created(){
    }
}
</script>

<style scoped>
    .width-40{
        max-width: 40vw;
    }
    img {
        width: 200px;
    }

    .company-title {
        color: white;
        font-size: 45px;
        text-align: center;
    }
</style>