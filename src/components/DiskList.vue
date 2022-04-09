<template>
    <div class="container">
        <div class="row">
            <div class="col-12 col-md-4 col-lg-3">
                <DiskItem/>
            </div>
        </div>
    </div>
</template>

<script>
import axios from 'axios';
import DiskItem from '@/components/DiskItem.vue';

export default {
    name: 'DiskList',
    data(){ 
        return{
            disks:[]
        }
    },
    props: {
        url: String
    },
    components: {
        DiskItem
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
                    if(response.status===200){
                        this.disks = response.data;
                        console.log(this.disks[0]);

                    }
                }
            )
        }
    }
}
</script>

<style lang="scss" scoped>

</style>