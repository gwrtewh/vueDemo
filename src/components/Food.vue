<template>
  <div class="Foot">
    <h1>选择你的食物</h1>
    <div class="dish" >
      <p class="dish_name">{{dish}}</p>
    </div>
    <button class="start_btn" type='button' @click='getStart()'>开始</button>
  </div>
</template>

<script>
import {foodList} from '../json/food.js';
export default {
  name: 'chooseFood',
  data () {
    return {
        foodList: foodList,
        dish: ""
    }
  },
  methods:{
    getStart(){
      
    }
  }
}
console.log(foodList);
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.dish{
/*  height: 300px;
  width: 300px;*/
  width: 150px;
  height: 150px;
  border: 1px solid #fff;
  margin: 10px auto;
  position: relative;
}
.dish_name{
  position: absolute;
  bottom: 50%;

  width: 100%;
  text-align: center;
}
.start_btn{
  margin-top: 30px;
}
/*h1, h2 {
  font-weight: normal;
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
}*/
</style>
