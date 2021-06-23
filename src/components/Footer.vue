<template>
  <div>
      <section id="link_section">
        <div>
            <img id="logo" src="../assets/img/footer-logo-1.png" alt="logo">
            <p>Providing Life Changing Experiences Through Education. Class That Fit Your Busy Life. Closer To Home</p>
            <div id="phone_number">
                <i class="fas fa-phone-alt">
                    <i class="fas fa-arrow-right"></i>
                </i>
                <span>1-677-124-44227</span>
            </div> <br>
            <div id="schedule">
                <i class="far fa-clock"></i>
                <span>Mon-Sat 8.00-18.00</span>
            </div>
        </div>
        <div>
            <h3>Popular Courses</h3>
            <ul>
                <li v-for="(element,index) in professors" :key="index">
                    <h4>{{ element.name }}</h4> 
                    <p>{{ element.subject }}</p>
                </li>
            </ul>
        </div>
        <div>
            <h3>Support</h3>
            <ul>
                <li v-for="(element,index) in support" :key="index">
                    <a href="#">{{ element }}</a>
                </li>
            </ul>
        </div>
        <div>
            <h3>Flexible Learning</h3>
            <img id="globo" src="../assets/img/footer-img-1.png" alt="">
        </div>
      </section>
      <section id="phone_contact_section">
          <div id="copyright">
              <p>Copyrights 2017 <i class="far fa-copyright"></i>Mikado Themes</p>
          </div>
          <div id="contact">
              <p>CALL +44 300 303 0266</p>
              <p id="foolow_us">Follow Us</p>
              <a href="">
                  <i class="fab fa-twitter"></i>
              </a>
              <a href="">
                  <i class="fab fa-instagram"></i>
              </a>
              <a href="">
                  <i class="fab fa-facebook-f"></i>
              </a>
          </div>
      </section>
  </div>
</template>

<script>
export default {
    name:'Footer',
    props:{
        professors:Array,
        support:Array
    }
}
</script>

<style lang="scss" scoped>

    div {
        width: 100%;
        background-color: #222222;

        #link_section {
            display: flex;
            justify-content: space-around;
            width: 90%;
            margin: 0 auto;
            padding: 120px 0 100px 0;

            & > div {
                width: calc(100% / 4);
                height: 100%;
                padding: 0 40px;

                #logo {
                    width: 50%;
                }

                h3 {
                    margin-bottom: 30px;
                    font-size: 25px;
                    font-weight: 400;
                    color: white;
                }

                & > p {
                    margin: 30px 0;
                    padding-right: 40px;
                    font-size: 14px;
                    line-height: 25px;
                    color: #A1A1A1;
                }

                #globo {
                    width: 70%;
                    cursor: pointer;
                }

                #phone_number {
                    .fa-phone-alt {
                        position: relative;
                        margin-right: 15px;

                        .fa-arrow-right {
                            position: absolute;
                            top: 0;
                            left: 10px;
                            font-size: 8px;
                            transform: rotate(140deg);
                        }
                    }
                }

                .fa-clock {
                    margin-right: 15px;
                }

                span {
                    font-size: 12px;
                    font-family: Arial, Helvetica, sans-serif;
                    color: white;
                }

                i {
                    color: #A1A1A1;
                    cursor: pointer;
                }
                i:hover {
                    color: #40C4FF;
                }

                ul {
                    list-style: none;
                    padding: 0;

                    li {
                        margin: 20px 0;

                        a {
                            text-decoration: none;
                            font-size: 15px;
                            cursor: pointer;
                            transition: 0.2s;
                            color: #A1A1A1;
                        }
                        a:hover {
                            color: #40C4FF;
                        }

                        h4 {
                            color: #CECECE;
                            transition: 0,2s;
                            cursor: pointer;
                        }
                        h4:hover {
                            color: #40C4FF;
                        }

                        & > p {
                            margin: 8px 0;
                            font-size: 14px;
                            cursor: pointer;
                            transition: 0.2s;
                            color: #A1A1A1;
                        }
                        & > p:hover{
                            color: #777575;
                        }
                    }

                }
            }
        }

        #phone_contact_section {
            display: flex;
            align-items: center;
            justify-content: space-between;
            width: 90%;
            margin: 0 auto;
            height: 100px;
            font-family: Arial, Helvetica, sans-serif;
            border-top: 2px solid #AAAAAA;

            #copyright {
                width: 50%;
                font-size: 15px;
                color: #828282; 
                cursor: pointer;
            }

            #contact {
                display: flex;
                align-items: center;
                justify-content: flex-end;
                width: 50%;
                color: #828282; 

                a {
                    color: #828282; 
                    margin: 0 0 0 20px;
                    cursor: pointer;
                    transition: 0.3s;
                }
                a:hover {
                    color: #40C4FF;
                }

                & > p {
                    margin: 20px;
                    font-size: 14px;
                }

                #foolow_us {
                    text-transform: uppercase;
                }

            }

        }
        
    }

</style>