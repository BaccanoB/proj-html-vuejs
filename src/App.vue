<template>
  <div id="app">
    <Header :nav="nav"/> 
    <Main :icons="icons"
    :images="images"
    :profiles="profiles"
    :list="list"/>
    <Footer :professors="professors"
    :support="support"/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

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
      nav:['Home','Courses','Instructors','Events','Pages','Elements'],  
      icons:[
        {
            'description': "Languages",
            'img':"https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-1.png"
        },
        {
            'description': "Software",
            'img':"https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-2.png"
        },
        {
            'description': "Business",
            'img':"https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-3.png"
        },
        {
            'description': "Chemistry",
            'img':"https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-4.png"
        },
        {
            'description': "Science",
            'img':"https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-5.png"
        },
        {
            'description': "DIY & Craft",
            'img':"https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-6.png"
        }
      ],
      images:[
        {
          'img':require('./assets/img/h5-client-5.png'),
          'imgHover':require('./assets/img/h5-client-5-h.png')
        },
        {
          'img':require('./assets/img/h5-client-1.png'),
          'imgHover':require('./assets/img/h5-client-1-h.png')
        },
        {
          'img':require('./assets/img/h5-client-2.png'),
          'imgHover':require('./assets/img/h5-client-2-h.png')
        },
        {
          'img':require('./assets/img/h5-client-1.png'),
          'imgHover':require('./assets/img/h5-client-1-h.png')
        }
      ],
      profiles:[
        {
          'img':require('./assets/img/course-5-f-img.jpg'),
          'name':'David Sanders',
          'subject':'Android Developer',
          'text':'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat vitae, a obcaecati harum voluptatibus distinctio?     Dolorum, dignissimos.',
          'type':'Programming',
          'cost':'Free'
        },
        {
          'img':require('./assets/img/course-6-f-img.jpg'),
          'name':'Jennifer Powell',
          'subject':'Web Designing',
          'text':'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat vitae, a obcaecati harum voluptatibus distinctio?     Dolorum, dignissimos.',
          'type':'Programming',
          'cost':'Free'
        },
        {
          'img':require('./assets/img/course-12-f-img.jpg'),
          'name':'Edward Bowman',
          'subject':'Financial Modeling',
          'text':'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat vitae, a obcaecati harum voluptatibus distinctio?     Dolorum, dignissimos.',
          'type':'Business',
          'cost':'$20'
        }
      ],
      list:['What We Do','Degree Program','Carrer Achivements','Personal Managment','Steps To Success','Knowledge Tranfer'
      ]
    }
  }  
}
</script>

<style lang="scss">

 @import './style/general';
</style>
