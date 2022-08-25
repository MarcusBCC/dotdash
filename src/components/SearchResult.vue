<template>
  <div class="card-form" style="margin-top: 10px">
    <li class="list-group-item">
    <div class = "row">
        <div class = "col-2" style="margin-right:50px;">
    <img :src="this.bookData.imageUrl">
    </div>
    <div class = "col">
    <h2>{{this.bookData.title}}</h2>
    <ul>
        <li>Author: {{this.bookData.authorName}}</li>
        <li>Rating: {{this.bookData.rating}}</li>
        <li>Year Published: {{this.bookData.year}}</li>
    </ul>
    

    </div>
    </div>
    </li>
  </div>
</template>

<script>
export default {
    
  name: "SearchResult",
  components: {},
  data() {
    return {
      
    };
  },
  props: {
    bookData:Object
    
  },
  methods: {
    
    
  },
};
</script>

<style>
</style>
