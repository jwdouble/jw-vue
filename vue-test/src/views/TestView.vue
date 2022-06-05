<template>
    <div>
        测试
        <!-- <router-link to="http://150.158.7.96:32056/health">
           axios
        </router-link> -->
        <button @click="TestAxios">axios</button>
    </div>
</template>

<script lang="ts">
import axios from 'axios'
export default{
    name:"Test",
    components:{

    },
    methods:{
        TestAxios(){
            axios.get("http://150.158.7.96:32056/health").then(function(data){
                console.log(data);
            }).catch(function(data){
                console.log(data);
            })
        }
    }
}
</script>

<style scoped>

</style>