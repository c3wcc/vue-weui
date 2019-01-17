<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
   
    <wv-button @click="aaa()"  type="primary" :mini="true">跳转</wv-button>
   
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "hello word"
    };
  },
  methods:{
    aaa(){
      console.log("44444")
      this.$router.push({
        path:'/aaa'
      })
      var obj = {
          pageSize: 20
      };

      // this.$http.get({url: '/api/ershou/my/delete_post' , params: obj })
      // .then((res) => {
      //   // 请求成功回调
      //     console.log(res)
      // }, () => {
      //   // 请求失败回调
      // });

      console.log("44444")

    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
