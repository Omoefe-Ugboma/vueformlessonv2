<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id">
    <router-link :to="{name:'JobDetails',params:{id:job.id}}">
        {{job.title}}
    </router-link>
    
  </div>
</template>

<script>
export default {
data(){
    return{
        jobs:[
            {title: 'Web developer', id:1, details:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident voluptates distinctio, assumenda nihil libero enim, a, nostrum aspernatur veritatis porro dolor consectetur laudantium? Accusamus minima labore esse minus, quasi necessitatibus.'},
            {title: 'Web designer', id:2, details:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident voluptates distinctio, assumenda nihil libero enim, a, nostrum aspernatur veritatis porro dolor consectetur laudantium? Accusamus minima labore esse minus, quasi necessitatibus.'},
            {title: 'Data Analyst', id:3, details:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident voluptates distinctio, assumenda nihil libero enim, a, nostrum aspernatur veritatis porro dolor consectetur laudantium? Accusamus minima labore esse minus, quasi necessitatibus.'},
        ]
    }
}
}
</script>

<style>

</style>template