<template>
  <h1>{{title}}</h1>
  <Modal :header="header" :text="text" theme="sale"/>
  <!--<input type="text" ref="name">
  <button @click="handleClick">click me</button>-->
</template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: 'App',
  components: { Modal },
  data(){
    return {
      title: 'My First Vue App',
      header: "Sign up for the giveaway!",
      text: "Grab your ninja swag for half price!"
    }
  },
  methods: {
    handleClick(){
      console.log(this.$refs.name)
      this.$refs.name.classList.add('active')
      this.$refs.name.focus()
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
h1 {
  border-bottom: Avenir, Helvetica, Arial, sans-serif;
  display: inline-block;
  padding-bottom: 10px;
}
</style>
<!--npm run serve -->
<!--https://github.com/Bilboking/Vue_SPA_project.git
git remote set-url origin https://github.com/Bilboking/Vue_SPA_project.git
git remote -v
git add .
git commit -m "Initial commit"
git push origin -u master

//git checkout -b "directory" or git branch testing <<- then ->> git push -u origin testing
//git add . 
//git commit -m "new branch message"
//git push -u origin branch
//git push origin branch-->