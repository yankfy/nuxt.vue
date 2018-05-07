<template>
  <div>
    <h1>姓名：{{info.name}}</h1>
    <h1>年龄：{{info.age}}</h1>
    <h1>兴趣：{{info.interest}}</h1>
  </div>
</template>

<script>
  import axios from 'axios'
  export default {
    data() {
      return {
        name: "Hello World"
      }
    },
    async asyncData() {
      let {
        data
      } = await axios.get('https://api.myjson.com/bins/r3cnm')
      return {
        info: data
      }
    }
    // asyncData() {
    //   return axios.get('https://api.myjson.com/bins/r3cnm')
    //     .then((res) => {
    //       console.log(res)
    //       return {
    //         info: res.data
    //       }
    //     })
    // } 
  }

</script>

<style>


</style>
