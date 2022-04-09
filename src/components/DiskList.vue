<template>
  <div class="disk"></div>
</template>

<script>
import axios from 'axios';

export default {
    name: 'DiskList',
    props: {
        url: String
    },
    mounted(){
        this.loadDiskData();
    },
    methods: {
        loadDiskData(){
            //axios restituisce promessa
            axios.get(this.url).then(
                (response)=>{
                    console.log(response);
                }
            )
        }
    }
}
</script>

<style lang="scss" scoped>

</style>