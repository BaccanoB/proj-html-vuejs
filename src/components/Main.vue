<template>
  <div >
    <!-- icon section -->
    <section id="icon_section">
        <div class="tx_align" v-for="(element,index) in icons" :key="index">
            <img class="cursor" :src="element.img" alt="language_img">
            <p>{{ element.description }}</p>
        </div>
    </section>
    <!-- /icon section -->

    <!-- trusted section -->
    <section id="trusted_name_section">
        <h2>The Trusted Name for In-Home Tutoring.</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit a autem eligendi ipsa architecto. Est rem aliquid incidunt fugit ducimus, minima architecto sequi eos iste earum. Neque dignissimos voluptate facilis?</p>
        <div>
            <a class="cursor uppercase" href="#">Learn More</a> 
            <i class="fas fa-chevron-right"></i>
        </div>
        <img src="../assets/img/h5-img-1.jpg" alt="people">
    </section>
    <!-- /trusted section -->

    <!-- empowering section -->
    <section id="empowering_section">
        <div>
            <img src="../assets/img/h1-img-8.jpg" alt="world">
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
        <div class="tx_align" id="student_profile">
            <img src="../assets/img/testimonials-standard-2.png" alt="student">
            <p>"Lorem ipsum dolor sit, amet consectetur adipisicing elit. Enim temporibus non, reiciendis architecto ipsum praesentium possimus quibusdam ullam? Velit nam exercitationem quas ipsam atque et voluptate amet dignissimos tenetur odio laudantium beatae vitae sequi, veritatis quibusdam repellendus ipsum natus officia."</p>
            <h4>Joan Collins</h4>
            <span class="uppercase">Student</span>
            <div id="dot_container">
                 <i
                    v-for="(image,index) in students" :key="index" 
                    :class="(index == indexImage) ? 'far' : 'fas'"
                    class="fa-circle cursor"
                    @click="goToImage(index)" 
                ></i>
            </div>

        </div>
    </section>
    <!-- /blu section -->

    <!-- learning section -->
    <section id="learning_section">
        <div id="learning_container">
            <div id="list">
            <ul>
                <li class="cursor" v-for="(item,index) in list" :key="index">
                    <a href="#">{{item}}</a>
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
    <section id="popular_section" class="tx_align">
        <h2>Popular Online Courses</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod, dolorum nisi architecto optio repellendus nemo. Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam, facilis. </p>
        <div id="slide_container">
            <div v-for="(element,index) in profiles" :key="index">
                <img class="cursor" :src="element.img" alt="img">
                <div class="slide_title">
                    <h4 class="cursor"> {{ element.subject }}</h4> 
                    <span class="free uppercase">{{ element.cost }}</span>
                </div>
                <h5>{{ element.name }}</h5>
                <p>{{element.text}}</p>
                <div>
                    <i class="fas fa-user"></i>
                    <span>1</span>
                    <i class="fas fa-tag"></i>
                    <span class="uppercase">{{ element.type }}</span>                    
                </div>
            </div>
        </div>
        <div id="dot_slide">
            <i v-for="(dot,index) in 3" :key="index" class="fas fa-circle"></i>
        </div>
    </section>
    <!--/ popular section -->

    <!-- pricing section -->
    <section id="pricing_plans_section" class="tx_align">
        <h2>Pricing Plans</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil, libero fugit. Aliquam corrupti facere fugiat.</p>
        <div id="tabel_container">
            <div>
                <h3 id="promo">Save up to 40% by paying weekly</h3>
                <ul>
                    <li>Number of Courses</li>
                    <li>Time</li>
                    <li>Web Designing</li>
                    <li>Human-Centered Design</li>
                    <li>Basic Marketing</li>
                    <li>Phyton For Everybody</li>
                    <li>Android Developer</li>
                    <li>Business English</li>
                </ul>
            </div>
            <div class="img_tabel_container tx_align">
                <img src="../assets/img/h5-custom-icon-7.png" alt="light">
                <h3>Standard</h3>
                <p>&#36;12</p>
                <ul>
                    <li>2</li>
                    <li>15 Days</li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-times"></i></li>
                    <li><i class="fas fa-times"></i></li>
                    <li><i class="fas fa-times"></i></li>
                    <li><i class="fas fa-times"></i></li>
                    <div class="button_container">
                        <button>Get it now</button>
                    </div>
                </ul>
            </div>
            <div class="img_tabel_container active_col tx_align" >
                <img src="../assets/img/h5-custom-icon-8.png" alt="brain">
                <h3>Professional</h3>
                <p>&#36;59</p>
                <ul>
                    <li>4</li>
                    <li>30 Days</li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-times"></i></li>
                    <li><i class="fas fa-times"></i></li>
                    <div class="button_container">
                        <button class="button_active">Get it now</button>
                    </div>
                </ul>
            </div>
            <div class="img_tabel_container tx_align">
                <img src="../assets/img/h5-custom-icon-9.png" alt="cart">
                <h3>Advanced</h3>
                <p>&#36;88</p>
                <ul>
                    <li>6</li>
                    <li>30 Days</li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-check"></i></li>
                    <li><i class="fas fa-check"></i></li>
                    <div class="button_container">
                        <button>Get it now</button>
                    </div>
                </ul>
            </div>
        </div>
    </section>
    <!-- /pricing section -->

    <!-- logo section -->
    <section id="logo_section">
        <div v-for="(element,index) in images" :key="index" >
            <img :src="hovered==false?element.img:element.imgHover" 
            @mouseover="hovered = true"
            @mouseleave="hovered=false"
            alt="logo">
        </div> 
    </section>
    <!-- /logo section -->

    <div id="top_square" class="cursor">
        <i class="fas fa-chevron-up "></i> 
        <p class="uppercase">Top</p>
    </div>
    <div id="logo">
        <img src="../assets/svg/svg-0.svg" alt="">
    </div>
    <div id="cart">
        <img src="../assets/svg/svg-2.svg" alt="">
    </div>
  </div>
</template>

<script>
export default {
    name:'Main',
    props:{
        icons:Array,
        images:Array,
        profiles:Array,
        list:Array
    },
    data(){
        return {
            hovered:false,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variable';
@import '../style/mixins';
    // icon
    #icon_section {
        @include flex;
        @include container;
        justify-content: center;
        flex-wrap: wrap;
        height: 400px;

        & > div {
            width: calc(100% / 7 );
            background-color:#F2F8FC;
            margin: 0 10px;
            padding: 40px 0;

            & > p {
                margin: 20px 0 10px 0;
                font-weight: bolder;
            }

            & > img {
                transition: 0.1s;
            }
            & > img:hover {
                transform: translateY(-5px);
            }
        }
    }
    // trusted
    #trusted_name_section {
        @include container;
        & > h2 {
            font-size: 40px;
            margin:  30px 925px 30px 0;
        }

        & > p {
            font-size: 18px;
            margin-bottom: 50px;
            color: #979797;
        }

        & > div{
            a {
                text-decoration: none;
                font-size: 15px;
                font-weight: bolder;font-family: Arial, Helvetica, sans-serif;
                color: $light_blu;
            }

            .fa-chevron-right {
                color: $light_blu;
                opacity: 0;
                font-size: 12px;
                margin-left: 3px;
            }
        }
        & > div:hover .fa-chevron-right{
            transition: 0.2s;
            opacity: 3;
            transform: translateX(6px);
        }

        & > img {
            margin-top: 40px;
            width: 90%;
        }
    }
    // empowering
    #empowering_section {
        display: flex;
        @include container;
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
                @include flex;
                flex-direction: row;
                width: 100%;
                margin-top: 60px;

                & > div {
                    .numbers {
                        font-size: 50px;
                        color: $light_blu;
                        margin: 25px 0;
                    }

                    & > p {
                        color: $light_blu;
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
            @include flex;
            @include container;
            flex-direction: column;
            height: 100%;
            padding: 100px;
            color: white;

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
        border-bottom: 2px solid $light_grey;

        #learning_container {
            display: flex;
            @include container;
            height: 100%;

            #list {
            width: 26%;
            height: 100%;
            margin-right: 60px;

            & > ul {
                list-style: none;
                
                & > li {
                    padding: 30px;
                    border: 1px solid $light_grey;
                    transition: 0.2s;

                    & > a {
                        text-decoration: none;
                        font-weight: bolder;
                        color: #989090;
                    }
                }
                & > li:hover {
                    border-left: 7px solid $light_blu;
                }
                & > li:hover a {
                    color: $light_blu;
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
                            color: $light_blu;
                        }
                    }
                }

                & > img {
                    position: absolute;
                    right: 5%;
                    bottom: 15%;
                    width: 18%;
                }
            }
        }
    }
    // popular
    #popular_section {
        width: 100%;
        padding: 100px 0;
        background-color: #F7F9F8;
        border-bottom: 2px solid $light_grey;

        & > h2 {
            font-size: 40px;
            margin: 20px 0;
            color: #303030;
        }

        & > p {
            margin: 5px 100px 80px 100px;
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
                border:1px solid $light_grey;
                transition: 0.2s;

                & > img {
                    width: 100%;
                }

                .slide_title {
                    @include flex;
                    justify-content: space-between;
                    padding-top: 30px;

                    & > h4 {
                        font-size: 18px;
                        color: #353535;
                        transition: 0.1s;
                    }
                    & > h4:hover {
                        color: $light_blu;
                    }

                    .free {
                        background-color: #ffd740;
                        color: white;
                        padding: 5px 10px;
                        border-radius: 40px;
                    }

                    #money {
                        background-color: $light_blu;
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
                        font-family: Arial, Helvetica, sans-serif;
                    }

                    .fa-tag {
                        margin-right: 5px;
                        transform: rotate(90deg);
                    }
                }
            }
             & > div:hover {
                 transform: translateY(-6px);
             }
        }
        

        #dot_slide {
            margin-top: 50px;
            & > i {
                margin: 5px;
                font-size: 13px;
                color: rgba(64, 196, 255, 0.5);
                cursor: pointer;
                transition: 0.1s;
            }
            & > i:hover {
                color: $light_blu;
            }
        }
    }
    // pricing
    #pricing_plans_section {
        width: 100%;
        padding:50px 50px 150px 50px;
        border-bottom: 2px solid $light_grey;

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

        #tabel_container {
            display: flex;
            @include container;

            .img_tabel_container {
                background-color: #F7FDFF;

                & > ul {
                    font-family: Arial, Helvetica, sans-serif;
                }
            }

            .active_col {
                border-top: 5px solid $light_blu;
            }

            & > div {
                width: calc(100% / 4);
                height: 100%;
                padding-top: 30px;
                text-align: left;
                border: 1px solid $light_grey;
                border-top: 5px solid rgba(64, 196, 255, 0.2);

                #promo {
                    padding: 95px 20px 75px 30px;
                    font-size: 25px;
                }

                & > h3 {
                    padding: 10px 0 20px 0;
                    font-size: 24px;
                    color: #303030;
                }

                & > p {
                    padding: 5px 0 20px 0;
                    font-family: Arial, Helvetica, sans-serif;
                    font-size: 20px;
                    font-weight: bolder;
                }

                & > ul {
                    list-style: none;

                    & > li {
                        padding: 30px;
                        font-weight: bolder;
                        font-size: 20px;
                        color: #989090;
                        border-top: 1px solid $light_grey;
                        border-bottom: 1px solid $light_grey;
                        background-color: white;

                        .fa-check {
                            color: $light_blu;
                        }
                    }
                }

            }

            .button_container {
                width: 100%;
                padding: 20px;
                background-color: #F7FDFF;

                & > button {
                    text-transform: uppercase;
                    font-weight: bolder;
                    color: #989090;
                    border: 2px solid $light_grey;
                    background-color: white;
                    padding: 20px 30px;
                    transition: 0.2s;
                    cursor: pointer;
                }

                & > button:hover {
                    color: white;
                    background-color: $light_blu;
                }

                .button_active {
                    color: white;
                    background-color: rgba(64, 196, 255, 0.7);
                }
            }
        }
    }
    // logo
    #logo_section {
        @include container;
        @include flex;
        justify-content: center;
        padding: 90px;
        cursor: pointer;
    }

    #top_square {
        position: fixed;
        top:50%;
        right: 0;
        @include flex;
        justify-content: center;
        flex-direction: column;
        width: 60px;
        height: 60px;
        font-weight: bolder;font-family: Arial, Helvetica, sans-serif;
        font-size: 13px;
        background-color: $light_blu;
        color: white;

        & > p {
            padding: 5px 0;
        }
        & > p:hover {
            display: none;
        }
    }


    #logo {
        @include flex;
        justify-content: center;
        position: fixed;
        top:33%;
        right: 0;
        width: 40px;
        height: 40px;
        background-color: #EF2853;

        & > img {
            width: 65%;
        }
    }

    #cart {
        @include flex;
        justify-content: center;
        border: 1px solid $light_grey;
        padding: 5px;
        position: fixed;
        top:40%;
        right: 0;
        width: 40px;
        height: 40px;
        background-color: white;

        & > img {
            width: 60%;
        }
    }


</style>