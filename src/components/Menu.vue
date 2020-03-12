<template>
  <div class="controle">
      <div class="menu">
          <ul>
              <li> <a href="#">Section 1</a></li>
              <li> <a href="#">Section 2</a></li>
              <li> <a href="#">Section 3</a></li>
              <li> <a href="#">Section 4</a></li>
          </ul>
      </div>
    <H2>{{ msg }}</H2>
  </div>
</template>

<script>
export default {
  name: 'Menu',
  props: {
    msg: String
  }
}
</script>
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
.link_header{
    float: right;
}
.menu{
  height: 45px;
  width: 99%;
  border: solid 2px;
  padding: 2px; 
}
</style>
