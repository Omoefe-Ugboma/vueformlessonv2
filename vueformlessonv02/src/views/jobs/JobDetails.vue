<template>
   <h1>Job Details Page</h1>
   <!-- <p>The job id is {{$route.params.id}}</p> -->
   <p>The job id is {{ id }}</p>
</template>

<script>
export default {
data(){
    return{
        //  props:['id'],
        id: this.$route.params.id
    }
}
}
</script>

<style>

</style>template