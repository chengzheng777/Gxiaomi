<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
    // import storage from './storage'

    export default { 
        name: 'app',
        components: {
            
        },
        data(){
            return {
                res: {}
            }
        },
        mounted(){
            // 本地加载请求静态json文件的形式
            // this.axios.get('/mock/user/login.json').then((res) => {
            //     this.res = res;
            // })
            // 通过easy-mock平台实现数据mock
            this.axios.get('/mock/user/login.json').then((res) => {
            this.res = res;
            })
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
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
