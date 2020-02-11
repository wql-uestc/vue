<template>
 <div class="add-event">
   <div v-if="!submited">
    <h2>添加活动</h2>
    <br>
    <label>活动标题</label>
    <input type="text" v-model="event.title">
    <br>
    <label>活动时间</label>
    <input type="text" v-model="event.time">
    <br>
    <label>活动地点</label>
    <input type="text" v-model="event.position">
    <br>
    <label>活动主要任务</label>
    <input type="text" v-model="event.assignment">
    <br>
    <label>活动主要内容</label>
    <textarea v-model="event.content"></textarea>
    <button v-on:click="addEvent">提交活动</button>
   </div>
   <label v-if="submited">事件提交成功</label>
  </div>
</template>

<script>
export default {
  name: 'add-event',
  data () {
    return {
      event:{
          title:'',
          time:'',
          position:'',
          assignment:'',
          content:''
      },
      submited:false
    }
  },
  methods:{
      addEvent(){
          this.submited=true;
          console.log(this.event);
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


</style>
