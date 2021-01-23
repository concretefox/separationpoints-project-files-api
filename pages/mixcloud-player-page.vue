<template>
    <div class ="w-100 container mx-auto">
        
    <MixcloudPlayer />




    </div>

</template>

<script>
// https://www.digitalocean.com/community/tutorials/how-to-use-vue-js-and-axios-to-display-data-from-an-api //
import MixcloudPlayer from '../components/MixcloudPlayer.vue'

const url = "https://min-api.cryptocompare.com/data/pricemulti?fsyms=BTC,ETH&tsyms=USD,EUR";

export default{
    components:  {
    MixcloudPlayer

    },

    data () {
    results: []
    return {

    }
    },

    mounted() {
    axios.get(url).then(response => {
    this.results = response.data

    })
    },


    
}

</script>