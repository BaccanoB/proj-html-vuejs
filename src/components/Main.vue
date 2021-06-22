<template>
  <div >
    <!-- icon section -->
    <section id="icon_section">
        <div>
            <img src="https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-1.png" alt="language_img">
            <p>Languages</p>
        </div>
        <div>
            <img src="https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-2.png" alt="softwere_img">
            <p>Software</p>
        </div>
        <div>
            <img src="https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-3.png" alt=""> 
            <p>Business</p>
        </div>
        <div>
            <img src="https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-4.png" alt="chemistry_img">
            <p>Chemistry</p>
        </div>
        <div>
            <img src="https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-5.png" alt="science_img">
            <p>Science</p>
        </div>
        <div>
            <img src="https://iacademy.qodeinteractive.com/wp-content/uploads/2017/05/h5-custom-icon-6.png" alt="craft_img">
            <p>DIY&amp;Craft</p>
        </div>
    </section>
    <!-- /icon section -->

    <!-- trusted section -->
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
    <!-- /trusted section -->

    <!-- empowering section -->
    <section id="empowering_section">
        <div>
            <img src="../assets/img/h1-img-8.jpg" alt="">
        </div>
        <div id="empowering_text">
            <h2>Empowering Children To Reach Their Potential</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia laudantium, dolorum repellendus adipisci iusto deleniti molestiae ab minima excepturi animi.</p>
            <div id="number_container">
                <div>
                    <p class="numbers">168</p>
                    <p>User Stories</p>
                </div>
                <div>
                    <p class="numbers">347</p>
                    <p>Events</p>
                </div>
            </div>
        </div>
    </section>
    <!-- /empowering section -->

    <!-- blu section -->
    <section id="blu_section">
        <div id="student_profile">
            <img src="../assets/img/testimonials-standard-2.png" alt="">
            <p>"Lorem ipsum dolor sit, amet consectetur adipisicing elit. Enim temporibus non, reiciendis architecto ipsum praesentium possimus quibusdam ullam? Velit nam exercitationem quas ipsam atque et voluptate amet dignissimos tenetur odio laudantium beatae vitae sequi, veritatis quibusdam repellendus ipsum natus officia."</p>
            <h4>Joan Collins</h4>
            <span>student</span>
            <div id="dot_container">
                <i v-for="(dot,index) in 3" :key="index" class="fas fa-circle"></i>
            </div>

        </div>
    </section>
    <!-- /blu section -->

    <!-- learning section -->
    <section id="learning_section">
        <div id="learning_container">
            <div id="list">
            <ul>
                <li class="active">
                    <a href="#">What We Do</a>
                </li>
                <li>
                    <a href="#">Degree Program</a>
                </li>
                <li>
                    <a href="#">Carrer Achivements</a>
                </li>
                <li>
                    <a href="#">Personal Managment</a>
                </li>
                <li>
                    <a href="#">Steps To Success</a>
                </li>
                <li>
                    <a href="#">Knowledge Tranfer</a>
                </li>
            </ul>
            </div>
            <div id="learning_text">
                <h2>Learning Possibilities</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur modi magni, reprehenderit tenetur quibusdam esse incidunt! Officiis eum deserunt impedit nostrum nemo porro similique voluptas necessitatibus sed at? Laboriosam magnam in, consequatur labore dignissimos ullam.</p>
                <ul>
                    <li><i class="fas fa-check"></i> We enrich lives through learning.</li>
                    <li><i class="fas fa-check"></i> Miximizing potential through individual attention.</li>
                    <li><i class="fas fa-check"></i> The trusted name for specialized training.</li>
                    <li><i class="fas fa-check"></i> Peaople teach.People learn.This is where they connect.</li>
                </ul>
                <img src="../assets/img/h12-tabs-icon-1.png" alt="tabs">
            </div>
        </div>
    </section>
    <!-- /learning section -->

    <!-- popular section -->
    <section id="popular_section">
        <h2>Popular Online Courses</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod, dolorum nisi architecto optio repellendus nemo. Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam, facilis. </p>
        <div id="slide_container">
            <div>
                <img src="../assets/img/course-5-f-img.jpg" alt="img">
                <div class="slide_title">
                    <h4>Android Developer</h4> 
                    <span class="free">Free</span>
                </div>
                <h5>David Sanders</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat vitae, a obcaecati harum voluptatibus distinctio? Dolorum, dignissimos.</p>
                <div>
                    <i class="fas fa-user"></i>
                    <span>1</span>
                    <i class="fas fa-tag"></i>
                    <span>Programming</span>                    
                </div>
            </div>
            <div>
                <img src="../assets/img/course-6-f-img.jpg" alt="img">
                <div class="slide_title">
                    <h4>Web Designing</h4>
                    <span class="free">Free</span>
                </div>
                <h5>Jennifer Powell</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat vitae, a obcaecati harum voluptatibus distinctio? Dolorum, dignissimos.</p>
                <div>
                    <i class="fas fa-user"></i>
                    <span>1</span>
                    <i class="fas fa-tag"></i>
                    <span>Programming</span>
                </div>
            </div>
            <div>
                <img src="../assets/img/course-12-f-img.jpg" alt="img">
                <div class="slide_title">
                    <h4>Financial Modeling</h4>
                    <span id="money">&#36;20</span>
                </div>
                <h5>Edward Bowman</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat vitae, a obcaecati harum voluptatibus distinctio? Dolorum, dignissimos.</p>
                <div>
                    <i class="fas fa-user"></i>
                    <span>1</span>
                    <i class="fas fa-tag"></i>
                    <span>Business</span>
                </div>
            </div>
        </div>
        <div id="dot_slide">
            <i v-for="(dot,index) in 3" :key="index" class="fas fa-circle"></i>
        </div>
    </section>
    <!--/ popular section -->

    <!-- pricing section -->
    <section id="pricing_plans_section"></section>
    <!-- /pricing section -->

    <!-- logo section -->
    <section id="logo_section"></section>
    <!-- /logo section -->
  </div>
</template>

<script>
export default {
    name:'Main'
}
</script>

<style lang="scss" scoped>
    // icon
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
            background-color:#F2F8FC;
            text-align: center;
            padding: 40px 0;

            & > p {
                margin: 20px 0 10px 0;
                font-weight: bolder;
            }
        }
    }
    // trusted
    #trusted_name_section {
        position: relative;
        width: 90%;
        margin: 0 auto;
        & > h2 {
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
    // empowering
    #empowering_section {
        display: flex;
        width: 90%;
        margin: 0 auto;
        padding: 50px 0 50px 0;

        div {
            width: 50%;
            display: flex;
            flex-direction: column;

            & > img {
                width: 50%;
                padding-top: 100px;
            }

            & > h2 {
                margin: 10px 0;
                font-size: 40px;
            }

            & > p {
                line-height: 25px;
                color: #868686;
            }
        } 

        #empowering_text {
            padding: 20px 100px 20px 20px;

            #number_container {
                display: flex;
                align-items: center;
                flex-direction: row;
                width: 100%;
                margin-top: 60px;

                & > div {
                    .numbers {
                        font-size: 50px;
                        color: #44C5FF;
                        margin: 25px 0;
                    }

                    & > p {
                        color: #44C5FF;
                        margin: 0;
                        font-size: 20px;
                        font-weight: bolder;
                    }
                }
                
            }
        }
    }
    // blu
    #blu_section {
        width: 100%;
        height: 700px;
        background-image: url('../assets/img/h5-parallax-img-1.png');
        background-size: cover;

        #student_profile {
            display: flex;
            align-items: center;
            flex-direction: column;
            width: 90%;
            height: 100%;
            margin: 0 auto;
            padding: 100px;
            color: white;
            text-align: center;

            & > img {
                width: 10%;
                margin-bottom: 70px;
            }

            & > p {
                padding: 10px 70px;
                line-height: 28px;
            }

            & > h4 {
                font-size: 24px;
                margin: 20px 0 10px 0;
            }

            & > span {
                text-transform: uppercase;
                font-size: 14px;
                font-weight: bolder;
            }

            #dot_container {
                margin: 40px;

                & > i {
                    margin: 0 5px;
                    color: rgba(225, 225, 225, 0.5);
                }
            }
        }
    }
    // learning
    #learning_section {
        width: 100%;
        padding: 150px  0;
        border-bottom: 2px solid #eeecec;

        #learning_container {
            display: flex;
            width: 90%;
            margin: 0 auto;
            height: 100%;

            #list {
            width: 26%;
            height: 100%;
            margin-right: 60px;

            & > ul {
                list-style: none;
                
                & > li {
                    padding: 30px;
                    border: 1px solid #eeecec;

                    & > a {
                        text-decoration: none;
                        font-weight: bolder;
                        color: #989090;
                    }
                }

                .active {
                    border-left: 7px solid #40C4FF;
                    & > a {
                        color: #40C4FF;
                    }
                    
                }
            }
            }

            #learning_text {
                position: relative;
                width: 50%;

                & > h2 {
                    margin: 10px 0;
                    font-size: 40px;
                    color: #303030;
                }

                & > p {
                    margin: 20px 0;
                    font-size: 16px;
                    line-height: 27px;
                    color: #818181;
                }

                & > ul {
                    margin-top: 60px;
                    list-style: none;

                    & > li {
                        margin: 25px 0;
                        color: #818181;

                        & > i {
                            margin-right: 10px;
                            color: #40C4FF;
                        }
                    }
                }

                & > img {
                    position: absolute;
                    right: 5%;
                    bottom: 10%;
                    width: 18%;
                }
            }
        }
    }
    // popular
    #popular_section {
        width: 90%;
        margin: 0 auto;
        padding: 100px 0;
        text-align: center;
        background-color: #F7F9F8;

        & > h2 {
            font-size: 40px;
            margin: 20px 0;
            color: #303030;
        }

        & > p {
            margin: 5px 50px 80px 50px;
            line-height: 25px;
            color: #989090;
        }

        #slide_container {
            display: flex;
            justify-content: center;

            & > div {
                text-align: left;
                width: 25%;
                padding-bottom: 10px;
                margin: 10px 20px;
                background-color: white;
                border:1px solid #eeecec;

                & > img {
                    width: 100%;
                }

                .slide_title {
                    display: flex;
                    justify-content: space-between;
                    align-items: center;
                    padding-top: 30px;

                    & > h4 {
                        font-size: 18px;
                        color: #353535;
                    }

                    .free {
                        text-transform: uppercase;
                        background-color: #ffd740;
                        color: white;
                        padding: 5px 10px;
                        border-radius: 40px;
                    }

                    #money {
                        text-transform: uppercase;
                        background-color: #40C4FF;
                        color: white;
                        padding: 5px 15px;
                        border-radius: 40px;
                    }

                   
                }

                & > h5 {
                    padding: 10px;
                    color: #DBDBDB;
                }

                & > p {
                    line-height: 25px;
                    font-size: 13px;
                    padding: 10px 40px 10px 10px;
                    color: #989090;
                }

                & > div {
                    padding: 10px;
                    color: #B9B9B9;
                    font-size: 12px;
                    font-weight: bolder;

                    & > i {
                        margin: 0 10px;
                    }

                    & > span {
                        text-transform: uppercase;
                        font-family: Arial, Helvetica, sans-serif;
                    }

                    .fa-tag {
                        margin-right: 5px;
                        transform: rotate(90deg);
                    }
                }
            }
        }

        #dot_slide {
            margin-top: 50px;
            & > i {
                margin: 5px;
                font-size: 13px;
                color: rgba(64, 196, 255, 0.5);
            }
        }
    }

</style>