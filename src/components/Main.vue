<template>
  <div >
      <section id="icon_section">
          <div>
              <img src="../assets/img/h1-slide-img-5.png" alt="language_img">
              <p>Languages</p>
          </div>
          <div>
              <img src="../assets/img/h1-slide-img-7.png" alt="softwere_img">
              <p>Software</p>
          </div>
          <div>
              <!-- <img src="../assets/img/h1-slide-img-" alt=""> -->
              <p>Business</p>
          </div>
          <div>
              <img src="../assets/img/h1-slide-img-4.png" alt="chemistry_img">
              <p>Chemistry</p>
          </div>
          <div>
              <img src="../assets/img/h1-slide-img-3.png" alt="science_img">
              <p>Science</p>
          </div>
          <div>
              <img src="../assets/img/h1-slide-img-6.png" alt="craft_img">
              <p>DIY&amp;Craft</p>
          </div>
      </section>
      <section id="trusted_name_section">
          <h2>The Trusted Name for In-Home Tutoring.</h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit a autem eligendi ipsa architecto. Est rem aliquid incidunt fugit ducimus, minima architecto sequi eos iste earum. Neque dignissimos voluptate facilis?</p>
          <a href="#">Learn More</a> <br>
          <img src="../assets/img/h5-img-1.jpg" alt="">
          <div id="top_square">
              <i class="fas fa-chevron-up"></i> 
              <p>Top</p>
          </div>
      </section>
      <section id="empowering_section"></section>
      <section id="blu_section"></section>
      <section id="learning_sec tion"></section>
      <section id="popular_section"></section>
      <section id="pricing_plans_section"></section>
      <section id="logo_section"></section>
  </div>
</template>

<script>
export default {
    name:'Main'
}
</script>

<style lang="scss" scoped>

    #icon_section {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        width: 90%;
        margin: 0 auto;
        height: 400px;

        & > div {
            width: calc(100% / 6 - 20px);
            height: 250px;
            background-color:#F2F8FC;
            text-align: center;

            & > img {
                margin-top: 30px;
            }

            & > p {
                margin: 20px 0 10px 0;
                font-weight: bolder;
            }
        }
    }

    #trusted_name_section {
        position: relative;
        width: 90%;
        margin: 0 auto;
        h2 {
            font-size: 40px;
            margin:  30px 925px 30px 0;
        }

        & > p {
            font-size: 18px;
            margin-bottom: 50px;
            color: #979797;
        }

        a {
            text-decoration: none;
            text-transform: uppercase;
            font-size: 15px;
            font-weight: bolder;font-family: Arial, Helvetica, sans-serif;
            color: #44C5FF;
        }

        & > img {
            margin-top: 40px;
            width: 90%;
        }

        #top_square {
            position: absolute;
            left: 101%;
            top: 65%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            width: 60px;
            height: 60px;
            font-weight: bolder;font-family: Arial, Helvetica, sans-serif;
            font-size: 13px;
            text-transform: uppercase;
            background-color: #40C4FF;
            color: white;

            & > p {
                padding: 5px 0;
            }
        }
    }

</style>