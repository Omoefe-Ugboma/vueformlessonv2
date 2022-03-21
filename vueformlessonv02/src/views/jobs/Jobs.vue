<template>
  <h1>Jobs</h1>
  <div v-for="job in jobs" :key="job.id" class="job">
    <router-link :to="{name:'JobDetails',params:{id:job.id}}">
       <h1>{{job.title}}</h1>
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
.job h2{
  background: #f4f4f4f4;
  padding: 20px;
  border-radius: 10px;
  margin: 10px auto;
  max-width: 600px;
  cursor: pointer;
  color: #444;
}
.job h2:hover{
  background: #ddd;
}
.job a{
  text-decoration: none;
}
</style>