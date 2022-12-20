<template>
  <img alt="Vue logo" src="./assets/me.jpg">
  <h1>{{firstname}} &nbsp; {{lastname}}</h1>
  <h3>{{nickname}}</h3>
  <h3>{{age}}</h3>
  <h3>{{tel}}</h3>
  <h3>{{room}}</h3>
  <h3>{{major}}</h3>
  <h3>{{school}}</h3>
  <h2>{{getFullname()}}</h2>
  <ul>
    <li>{{hobby[0]}}</li>
    <li>{{hobby[1]}}</li>
    <li>{{hobby[2]}}</li>
    <li>{{hobby[3]}}</li>
    <li>{{hobby[4]}}</li>
  </ul>
  <ul>
    <li>{{profile.gender}}</li>
    <li>{{profile.hight}}</li>
  </ul>
</template>

<script>


export default {
  name: 'App',
  data(){
    return{
      firstname:"Sayaphorn",
      lastname:"Hlongthong",
      nickname:"faii",
      age:"19",
      tel:"0955231708",
      room:"IT5102",
      major:"Information Technology",
      school:"Lanna Polytechnic ChiangMai",
      hobby:["เล่นเกม","นอน","กิน","เหม่อ","เที่ยว"],
      profile:{gender:"female",weight:70,hight:160,status:false}
    }
  },
  methods : {
    getFullname(){
      return this.firstname + this.lastname
    }
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
