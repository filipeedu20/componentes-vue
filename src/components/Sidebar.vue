<template>
  <div class="sidebar">
      <div class="link_header">
          <ul>
              <li v-for="link in links" v-bind:key="link.text">
                  {{ link.text }}
              </li>              
          </ul>
      </div>
  </div>
</template>

<script>
export default {
  name: "",
 data(){
   return{
     links:[
       {text: "Section 1"},
       {text: "Section 2"},
       {text: "Section 3"},
       {text: "Section 4"}
     ]
   };
 }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.sidebar{
    height: 800px;
    width: 300px;
    float: right;
    text-align: left;
    padding-left:10px;
    border: solid 1px #cccccc;
    margin-right: 10px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  margin: 0 10px;
}
</style>
