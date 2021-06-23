<template>
  <div id="app">
    <Header :nav="nav" />
    <Main />
    <Footer :professors="professors"
    :support="support"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  },
  data(){
    return{
      professors:[
        {
          "name":"Preston Marshall",
          "subject":"Business English"
        },
        {
          "name":"David Sanders",
          "subject":"Social Computing"
        },
        {
          "name":"Jennie King",
          "subject":"Learn Spanish"
        }
      ],
      support:['User dashboard','Contact Us','FAQ','Course Offer','Events'],
      nav:['Home','Courses','Instructors','Events','Pages','Elements']
        
    }
  }
      // images:[
      //   {
      //     "img":"../assets/img/h5-client-5.png",
      //     'imgHover':"../assets/img/h5-client-5-h.png"
      //   },
      //   {
      //     'img':"../assets/img/h5-client-1.png",
      //     'imgHover':"../assets/img/h5-client-1-h.png"
      //   },
      //   {
      //     'img':"../assets/img/h5-client-2.png",
      //     'imgHover':"../assets/img/h5-client-2-h.png"
      //   },
      //   {
      //     'img':"../assets/img/h5-client-1.png",
      //     'imgHover':"../assets/img/h5-client-1-h.png"
      //   }
      // ]  
}
</script>

<style lang="scss">
@import './style/general';
</style>
