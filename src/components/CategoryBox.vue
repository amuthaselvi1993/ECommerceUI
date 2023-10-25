<template>
    <div class="card w-75 h-85" style = "margin-top: 3px">
        <div class ="embed-responsive embed-responsive-16by">
        <img 
         :src="category.imageUrl" 
         class="card-img-top" 
         alt="Card image cap"/>
        </div>
        <div class="card-body">
        <h4 class="card-title">{{ category.categoryName }}</h4>
        <p class="card-text">{{ category.description }}</p>
       <a href="#" class="btn btn-primary">Go somewhere</a> 
        </div> 
    </div>

</template>
<script>
//import { defineComponent } from '@vue/composition-api';
export default {
    name: "CategoryBox",
    props: ["category"],
    methods: {},
};
</script>

<style scoped>
.card-img-top {
    object-fit: cover;
}
</style>