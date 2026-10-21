<template>
    <div id="hero">
        <section class="hero">
            <div class="container">
                <div class="left">
                    <div class="img-wrap"><img src="@\assets\img\graphic\taro_promo.jpg" alt="Coffee" /></div>
                </div>
                <div class="split"></div>
                <div class="right">
                    <h1><span style="color: #8c62cf">Chill</span> with some milk.</h1>
                    <h1><span style="color: #8c62cf">Chill</span> like a panda.</h1>
                    <button @click="$router.push('noncoffee')">Explore Milk Series!</button>
                    <!--Learned this button trick from https://stackoverflow.com/questions/45638239/enclosing-a-router-link-tag-in-a-button-in-vuejs-->
                </div>
            </div>
        </section>
    </div>
</template>

<style scoped>
.container {
    overflow-x: hidden;
    overflow-y: hidden;
    width: 100%;
    height: 800px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    background-color: #8c62cf;
    background-color: #aa82cb;
    background-image: url('@/assets/img/background/taro_bubble_bg.png');
    background-position: 0px 0px;
    align-content: center;

    .left {
        display: flex;
        align-items: center;

        .img-wrap {
            width: 800px;
            height: 800px;
            display: flex;
            align-items: center;
            justify-content: center;

            img {
                width: 575px;
                rotate: 0deg;
                transition:
                    width 0.75s cubic-bezier(0.42, 0, 0, 1.32),
                    rotate 1s cubic-bezier(0.42, 0, 0, 1.32);
            }

            img:hover {
                width: 600px;
                rotate: -2deg;
            }
        }
    }

    .split {
        width: 50px;
    }

    .right {
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
            background: rgb(243, 255, 243);
            border-radius: 10px;
            color: #8c62cf;
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
        width: 100%;
        height: 800px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        background-color: #8c62cf;
        background-color: #aa82cb;
        background-image: url('@/assets/img/background/taro_bubble_bg.png');
        background-position: 0px -100px;
        align-content: center;
        text-align: center;

        .left {
            display: none;
            align-items: center;
            padding-right: 0px;

            .img-wrap {
                width: 100%;
                height: 800px;
                display: flex;
                align-items: center;
                justify-content: center;

                img {
                    width: 400px;
                    rotate: 0deg;
                    transition:
                        width 0.75s cubic-bezier(0.42, 0, 0, 1.32),
                        rotate 1s cubic-bezier(0.42, 0, 0, 1.32);
                }

                img:hover {
                    width: 450px;
                    rotate: -2deg;
                }
            }
        }

        .split {
            width: 50px;
        }

        .right {
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
                background: rgb(243, 255, 243);
                border-radius: 10px;
                color: #8c62cf;
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
