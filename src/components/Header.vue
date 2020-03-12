<template>
  <div class="header">
      <div class='img_header'>
      </div>
      <div class="link_header">
          <ul>
              <li v-for="link in links" v-bind:key="link.text">
                  {{ link.text }}
              </li>
              
          </ul>
      </div>
      <div class="search_header">
        <input type="text" text='Search' class='search'>
      </div>
  </div>
</template>
<script>
export default {
  name: "ListLinks",
 data(){
   return{
     links:[
       {text: "Topic 1"},
       {text: "Topic 2"},
       {text: "Topic 3"},
       {text: "Topic 4"}
     ]
   };
 }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.header{
    height: 200px;
    margin-top: 120px;
    padding: 20px;
}
.link_header{
    float: right;
    margin-top:-80px;
}
.img_header{
  background: red;
  height: 80px;
  width: 200px;
  margin-top:-100px;
  margin-left: 40px;
}
.search_header{
  float: right;
  margin-right: 10px;
  margin-top:70px;
}
.search{
  height: 40px;
  width: 300px;
}

</style>
