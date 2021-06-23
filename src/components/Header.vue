<template>
    <div id="container">
        <div id="transparency">
            <div id="header_bar">
                <img src="../assets/img/logo-light.png" alt="logo">
                <nav>
                    <ul>
                        <li v-for="(element,index) in nav" :key="index">
                            <a href="#">{{element}}</a>
                        </li>
                    </ul>
                </nav>
                <div id="icons">
                    <i class="fas fa-search"></i>
                    <i class="far fa-clipboard">
                        <div id="carel">0</div>
                    </i>
                    <i class="fas fa-bars"></i>
                </div>
            </div>
            <section>
                <h1>Contemporary Ideas</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit aliquam, aliquid eius sit veniam illo dolorum blanditiis, nostrum, tempora fugiat asperiores aperiam quis pariatur assumenda obcaecati.</p>
                <button>Register Now</button>
                <div id="circle">
                    <i v-for="(circle,i) in 2" :key="i" class="fas fa-circle"></i>
                    <i class="far fa-dot-circle"></i>
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
    }
}
</script>

<style lang="scss" scoped>
    #container {
        width: 100%;
        height: 700px;
        background-image: url('../assets/img/course-9-f-img.jpg');
        background-size: cover;
        background-position: center;  
        color: white;

        #transparency {

            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.3);

            #header_bar {
            width: 100%;
            height: 90px;
            display: flex;
            align-items: center;
            justify-content: space-between;

                & > img {
                    width: 15%;
                    padding-left: 50px;
                }

                nav {
                    width: 60%;
                    height: 100%;
                    display: flex;
                    align-items: center;
                    justify-content: center;

                    ul {
                        list-style: none;

                        li {
                            display: inline-block;
                            padding: 0 20px;

                            a {
                                color: white;
                                text-decoration: none;
                                text-transform: uppercase;
                                font-size: 15px;
                                transition: 0.1s;
                                cursor: pointer;
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
                    display: flex;
                    align-items: center;
                    justify-content: center;

                    i {
                        margin: 0 20px ;
                        font-size: 20px;
                        transition: 0.1s;
                        cursor:pointer;
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
                            display: flex;
                            align-items: center;
                            justify-content: center;
                            width: 12px;
                            height: 12px;
                            border-radius: 60%;
                            background-color: #40C4FF;
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
                    text-transform: uppercase;
                    font-weight: bolder;
                    background-color: #40C4FF;
                    border: 1px solid #40C4FF;
                    color: white;
                }

                #circle {
                    display: flex;
                    align-items: center;
                    justify-content: center;
                    margin-top: 90px;

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