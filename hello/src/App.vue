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
    
            }
        },
        mounted(){
           
        }
    }
</script>

<style>
@import './assets/scss/reset.scss'
</style>
