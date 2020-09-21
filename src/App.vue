<template>
    <div id="app">
    </div>
</template>

<script>

    export default {
        name: 'app',
        components: {

        },
        created(){
            // console.log(process.env.VUE_APP_DOMAIN);
            console.log(process.env.VUE_APP_API);
            $.get("/api/home/index/slide?token=1ec949a15fb709370f",(res)=>{
                console.log(res);
            });

        }
    }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
