<template>
    <div id="hero">
        <section class="hero">
            <div class="container">
                <div class="mobile-top">
                    <div class="img-mobile">
                        <img src="@\assets\img\graphic\hero_coffee.png" alt="Coffee" class="coffee-img-mobile" />
                    </div>
                </div>
                <div class="left">
                    <h1><span style="color: #4fb315">Boost</span> for your energy.</h1>
                    <h1><span style="color: #4fb315">Boost</span> for your budget.</h1>
                    <button @click="$router.push('coffee')">Explore Coffee Series!</button>
                    <!--Learned this button trick from https://stackoverflow.com/questions/45638239/enclosing-a-router-link-tag-in-a-button-in-vuejs-->
                </div>
                <div class="split"></div>
                <div class="right">
                    <div class="right-bg">
                        <div class="img-wrap">
                            <img src="@\assets\img\graphic\hero_coffee.png" alt="Coffee" class="coffee-img" />
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<style scoped>
.hero {
    width: 100%;
    height: 800px;
    margin: 0px;
}

.container {
    overflow-x: hidden;
    overflow-y: hidden;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-content: center;
    background-color: rgb(136, 218, 92);
    background-image: url('@/assets/img/background/green_bubble_bg.png');
    background-position: 0px -200px;

    .img-mobile {
        display: none;
    }

    .right {
        display: flex;
        align-items: center;
        padding-right: 50px;

        .right-bg {
            align-items: center;
            justify-content: center;
            width: 800px;
            height: 800px;
            clip-path: polygon(100% 0%, 80% 100%, 0% 100%, 20% 0%);
            /**https://www.cssportal.com/css-clip-path-generator/**/
            background-color: rgb(176, 255, 133);

            .img-wrap {
                width: 800px;
                height: 800px;
                display: flex;
                align-items: center;
                justify-content: center;

                .coffee-img {
                    width: 600px;
                    rotate: 0deg;

                    transition:
                        width 0.75s cubic-bezier(0.42, 0, 0, 1.32),
                        rotate 1s cubic-bezier(0.42, 0, 0, 1.32);
                    /**https://www.cssportal.com/css-cubic-bezier-generator/**/
                }

                .coffee-img:hover {
                    rotate: -10deg;
                    width: 700px;
                }
            }
        }
    }

    .split {
        width: 10px;
    }

    .left {
        margin-left: 50px;
        display: block;
        align-content: center;
        justify-content: center;
        line-height: 100px;

        h1 {
            font-size: 60px;
            line-height: 50px;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            color: #f5f5f5;
        }

        h2 {
            font-weight: lighter;
            font-family: Arial, Helvetica, sans-serif;
            line-height: 0px;
        }

        button {
            width: 400px;
            height: 60px;
            font-size: 30px;
            border: 0;
            padding: 10px;
            z-index: 100;
            background: rgb(243, 255, 243);
            border-radius: 10px;
            color: #4fb315;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            cursor: pointer;
            box-shadow: 0px 0px 10px 0px #4d714c63;
            transition:
                width 0.25s,
                height 0.25s,
                font-size 0.5s,
                box-shadow 0.5s;
        }

        button:hover {
            box-shadow: 0px 0px 20px 5px #4d714c63;
            width: 410px;
            height: 70px;
            font-size: 32px;
        }
    }
}

@media (max-width: 768px) {
    .container {
        margin-left: 0px;

        padding-top: 0px;
        width: 100%;
        height: 1000px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-content: center;
        text-align: center;
        background-position: 0px 0px;

        .mobile-top {
            display: flex;
            align-items: center;
            justify-content: center;

            .img-mobile {
                width: 100px;
                height: 100px;
                display: flex;
                align-items: center;
                justify-content: center;

                .coffee-img-mobile {
                    width: 300px;
                    rotate: 0deg;

                    transition:
                        width 0.75s cubic-bezier(0.42, 0, 0, 1.32),
                        rotate 1s cubic-bezier(0.42, 0, 0, 1.32);
                    /**https://www.cssportal.com/css-cubic-bezier-generator/**/
                }

                .coffee-img-mobile:hover {
                    rotate: -10deg;
                    width: 350px;
                }
            }
        }

        .right {
            display: none;
            align-items: center;
            padding-right: 0px;

            .right-bg {
                display: none;
                align-items: center;
                justify-content: center;
                width: 100%;
                height: 300px;
                clip-path: none;
                background-color: rgb(176, 255, 133, 000);

                .img-wrap {
                    width: 800px;
                    height: 800px;
                    display: flex;
                    align-items: center;
                    justify-content: center;


                    .coffee-img {
                        width: 400px;
                        rotate: 0deg;
                        display: none;
                        transition:
                            width 0.75s cubic-bezier(0.42, 0, 0, 1.32),
                            rotate 1s cubic-bezier(0.42, 0, 0, 1.32);
                        /**https://www.cssportal.com/css-cubic-bezier-generator/**/
                    }

                    .cofee-img:hover {
                        rotate: -10deg;
                        width: 450px;
                    }
                }
            }
        }

        .split {
            width: 10px;
        }

        .left {
            margin: 0px;
            padding: 0px;
            display: block;
            align-content: center;
            justify-content: center;
            height: 500px;
            line-height: 100px;
            padding-left: 0px;

            h1 {
                font-size: 60px;
                line-height: 50px;
                font-family: Verdana, Geneva, Tahoma, sans-serif;
                color: #f5f5f5;
            }

            h2 {
                font-weight: lighter;
                font-family: Arial, Helvetica, sans-serif;
                line-height: 0px;
            }

            button {
                width: 400px;
                height: 60px;
                font-size: 30px;
                border: 0;
                padding: 10px;
                background: rgb(243, 255, 243);
                border-radius: 10px;
                color: #4fb315;
                font-family: Verdana, Geneva, Tahoma, sans-serif;
                cursor: pointer;
                box-shadow: 0px 0px 10px 0px #4d714c63;
                transition:
                    width 0.25s,
                    height 0.25s,
                    font-size 0.5s,
                    box-shadow 0.5s;
            }

            button:hover {
                box-shadow: 0px 0px 20px 5px #4d714c63;
                width: 410px;
                height: 70px;
                font-size: 32px;
            }
        }
    }
}
</style>
