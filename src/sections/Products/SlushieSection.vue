<template>
    <div id="Slushie">
        <section class="Slushie">
            <div class="container">
                <div class="title">
                    <h1>Slushie Series</h1>
                    <div class="price">
                        <h3>₱59/₱69</h3>
                    </div>
                    <h2>w/ Nata</h2>
                </div>
                <div class="items">
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap">
                                <img src="@/assets/img/product/noncoffee/Slushie.png" alt="Slushie Series" />
                            </div>
                        </div>
                    </div>

                    <div class="card-space wide">
                        <div class="card">
                            <div class="series-list">
                                <p class="series-item">· Strawberry</p>
                                <p class="series-item">· Kiwi</p>
                                <p class="series-item">· Passion Fruit</p>
                                <p class="series-item">· Blueberry</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<style scoped>
.container {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-items: center;
    align-items: center;
    background: radial-gradient(circle,
            rgba(230, 253, 255, 1) 0%,
            rgba(245, 245, 245, 1) 25%,
            rgba(245, 245, 245, 1) 43%,
            rgba(217, 253, 255, 1) 55%,
            rgba(240, 251, 255, 1) 77%,
            rgba(227, 249, 255, 1) 100%);
    padding-bottom: 50px;
    padding-top: 100px;

    .title {
        display: flex;
        flex-direction: column;
        justify-items: center;
        align-items: center;
        text-align: center;
        line-height: 20px;
        padding-bottom: 50px;
        line-height: 0px;

        h1 {
            font-size: 80px;
            font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
            color: #222267;
        }

        h2 {
            font-size: 30px;
            line-height: 30px;
            font-family: Arial, Helvetica, sans-serif;
            color: #3b3bba;
        }

        .price {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 300px;
            height: 75px;
            font-size: 50px;
            font-family: Arial, Helvetica, sans-serif;
            background-color: #222267;
            color: #f5f5f5;
            border-radius: 30px;
        }
    }

    .items {
        display: grid;
        grid-template-columns: 1fr;
        justify-items: center;
        gap: 50px;
        width: 100%;

        .card-space {
            width: 500px;
            height: auto;
            place-content: center;
            display: flex;

            .card {
                width: 500px;
                height: 300px;
                display: flex;
                flex-direction: column;
                place-items: center;
                background-color: #f5f5f5;
                border-radius: 20px;
                box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 15px 0px;
                padding: 25px;
                font-family: Arial, Helvetica, sans-serif;
                line-height: 0px;

                .image-wrap {
                    width: 100%;
                    height: 100%;
                    align-items: center;
                    place-content: center;
                    display: flex;
                }

                img {
                    width: 450px;
                    place-items: center;
                    transition: width 0.25s;
                    transition-timing-function: cubic-bezier(0.42, 0, 0.31, 1.03);
                }

                img:hover {
                    width: 500px;
                }
            }
        }


        .card-space.wide {
            width: 100%;
            height: auto;
            place-content: center;
            padding-bottom: 0px;

            .card {
                width: fit-content;
                height: auto;
                padding: 40px 70px;
                line-height: 1.6;
                place-items: center;

                .series-list {
                    margin: 0;
                    padding: 0;
                    display: grid;
                    grid-template-columns: auto auto;
                    justify-content: center;
                    gap: 14px 60px;
                    text-align: left;

                    .series-item {
                        margin: 0;
                        font-size: 24px;
                        font-weight: bold;
                        color: #222267;
                        white-space: nowrap;
                    }
                }
            }
        }
    }
}

@media (max-width: 768px) {
    .container {
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-items: center;
        align-items: center;
        text-align: center;
        background-color: #ffffffca;
        padding-top: 150px;

        .title {
            display: flex;
            flex-direction: column;
            justify-items: center;
            align-items: center;
            text-align: center;
            line-height: 20px;
            padding-bottom: 50px;
            line-height: 0px;

            h1 {
                font-size: 60px;
                font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
                color: #222267;
            }

            h2 {
                font-size: 25px;
                line-height: 30px;
                font-family: Arial, Helvetica, sans-serif;
                color: #3b3bba;
            }

            .price {
                display: flex;
                align-items: center;
                justify-content: center;
                width: 200px;
                height: 50px;
                font-size: 30px;
                font-family: Arial, Helvetica, sans-serif;
                background-color: #222267;
                color: #f5f5f5;
                border-radius: 30px;
            }
        }

        .items {
            display: grid;
            grid-template-columns: 1fr;
            justify-items: center;
            gap: 50px;
            width: 100%;

            .card-space {
                width: 500px;
                height: auto;
                place-content: center;
                display: flex;

                .card {
                    width: 500px;
                    height: 300px;
                    display: flex;
                    flex-direction: column;
                    place-items: center;
                    background-color: #f5f5f5;
                    border-radius: 20px;
                    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 15px 0px;
                    padding: 25px;
                    font-family: Arial, Helvetica, sans-serif;
                    line-height: 0px;

                    .image-wrap {
                        width: 100%;
                        height: 100%;
                        align-items: center;
                        place-content: center;
                        display: flex;
                    }

                    img {
                        width: 450px;
                        place-items: center;
                        transition: width 0.25s;
                        transition-timing-function: cubic-bezier(0.42, 0, 0.31, 1.03);
                    }

                    img:hover {
                        width: 500px;
                    }
                }
            }

            .card-space.wide {
                width: 100%;
                height: auto;
                place-content: center;
                padding-bottom: 0px;

                .card {
                    width: fit-content;
                    height: auto;
                    padding: 20px 70px;
                    line-height: 1.6;
                    place-items: center;

                    .series-list {
                        margin: 0;
                        padding: 0;
                        display: grid;
                        grid-template-columns: auto auto;
                        justify-content: center;
                        gap: 14px 60px;
                        text-align: left;

                        .series-item {
                            margin: 0;
                            font-size: 18px;
                            font-weight: bold;
                            color: #222267;
                            white-space: nowrap;
                        }
                    }
                }
            }
        }
    }
}
</style>
