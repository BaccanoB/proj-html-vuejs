<template>
    <div id="container">
         <div id="bg_img_container" v-for="i in [index]" :key="i">
            <img :src="currentImg" />
        </div>
        <div id="transparency">
            <div id="header_bar">
                <img src="../assets/img/logo-light.png" alt="logo">
                <nav>
                    <ul>
                        <li v-for="(element,index) in nav" :key="index">
                            <a class="cursor uppercase" href="#">{{element}}</a>
                        </li>
                    </ul>
                </nav>
                <div id="icons">
                    <i class="fas fa-search cursor"></i>
                    <i class="far fa-clipboard cursor">
                        <div id="carel">0</div>
                    </i>
                    <i class="fas fa-bars cursor"></i>
                </div>
            </div>
            <section>
                <h1>Contemporary Ideas</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit aliquam, aliquid eius sit veniam illo dolorum blanditiis, nostrum, tempora fugiat asperiores aperiam quis pariatur assumenda obcaecati.</p>
                <button class="uppercase cursor">Register Now</button>
                <div id="circle">
                    <i
                    v-for="(image,index) in bgImages" :key="index" 
                    :class="(index == indexImage) ? 'far fa-dot-circle' : 'fas fa-circle'"
                    class="far cursor"
                    @click="goToImage(index)" 
                    ></i>
                </div>
            </section>
        </div>
    </div>
</template>

<script>
export default {
    name:'Header',
    props: {
        nav:Array 
    },
    data(){
        return {
            bgImages:[
                {
                    'img':require('../assets/img/h5-slide-3-background.jpg')
                },
                {
                    'img':require('../assets/img/h5-slide-2-background.jpg')
                },
                {
                    'img':require('../assets/img/h5-slide-1-background.jpg')
                }
            ],
            indexImage:0
        }
    },
    computed: {
        currentImg: function() {
            let index = this.indexImage;
            return this.bgImages[index].img;
        }
    },
    methods:{
        goToImage: function(newIndex){
            this.indexImage = newIndex;
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variable';
@import '../style/mixins';
    #container {
        position: relative;
        width: 100%;
        height: 700px;
        color: white;

        #bg_img_container{
            width: 100%;
            height: 700px;

            & > img {
                width: 100%;
                height: 700px;
            }
        }
        

        #transparency {
            position: absolute;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.3);

            #header_bar {
            width: 100%;
            height: 90px;
            @include flex;
            justify-content: space-between;

                & > img {
                    width: 15%;
                    padding-left: 50px;
                }

                nav {
                    width: 60%;
                    height: 100%;
                    @include flex;
                    justify-content: center;

                    ul {
                        list-style: none;

                        li {
                            display: inline-block;
                            padding: 0 20px;

                            a {
                                color: white;
                                text-decoration: none;
                                font-size: 15px;
                                transition: 0.1s;
                            }

                            a:hover {
                                color: #dfdbdb;
                            }
                        }
                    }
                }

                #icons {
                    width: 20%;
                    height: 100%;
                    @include flex;
                    justify-content: center;

                    i {
                        margin: 0 20px ;
                        font-size: 20px;
                        transition: 0.1s;
                    }
                    i:hover {
                        color: #dfdbdb;
                    }

                    .fa-clipboard {
                        font-size: 22px;
                        position: relative;

                        #carel{
                            position: absolute;
                            top: 0;
                            left: 50%;
                            @include flex;
                            justify-content: center;
                            width: 12px;
                            height: 12px;
                            border-radius: 60%;
                            background-color: $light_blu;
                            font-size: 11px;
                        }

                    }

                    .fa-search {
                        transform: rotate(90deg);
                    }
                }
            }

            section {
                height: calc(100% - 90px);
                width: 70%;
                margin: 0 auto;
                padding-top: 100px;
                text-align: center;

                h1 {
                    font-size: 70px;
                    margin: 20px;
                }
                
                & > p {
                    padding: 10px;
                    font-size: 20px;
                    font-weight: 200;
                    line-height: 40px;
                    color: #FFFFFFCC;
                }

                button {
                    margin: 50px;
                    padding: 20px 40px;
                    font-weight: bolder;
                    background-color: $light_blu;
                    border: 1px solid $light_blu;
                    color: white;
                }

                #circle {
                    @include flex;
                    justify-content: center;
                    transition: 0.2s;

                    & > i {
                        margin: 0 8px;
                        color: rgba(225,225,225, 0.6);
                    }

                    .fa-dot-circle {
                        color: white;
                        font-size: 20px;
                    }
                }
            }
        }
    }

</style>