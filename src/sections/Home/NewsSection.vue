<template>
    <div id="home_news">
        <section class="home_news">
            <div class="container">
                <div class="title">
                    <h1>News</h1>
                </div>
                <div class="items">
                    <!--News 1-->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\news\event-volumens-26.avif" alt="atrolab37">
                            </div>
                            <h2>Volumens Festival</h2>
                            <p>Join renowned artist HD Substance for an inspiring masterclass on synthesis and sound
                                design at Volumens Festival, one of Spain's premier electronic and experimental music
                                artists.</p>
                            <div class="date-text">
                                <h3>16/10/2026</h3>
                            </div>
                        </div>
                    </div>
                    <!--News 2-->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\news\news-minifreak5-sm.avif"
                                    alt="atrolab37"></div>
                            <h2>Minifreak | New Firmware 5.0</h2>
                            <p>This free update adds user sample and wavetable import, plus a new Factory Bank v5.0 with
                                23 new presets</p>
                            <div class="date-text">
                                <h3>22/9/2026</h3>
                            </div>
                        </div>
                    </div>
                    <!--News 3-->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\news\news-audiofusestudiorev2-sm.avif"
                                    alt="atrolab37"></div>
                            <h2>AudioFuse Studio Rev2 | Premium Desktop Audio</h2>
                            <p>Discover AudioFuse Studio in an elevated Rev2 edition, featuring optimized preamps and an
                                updated Bluetooth module.</p>
                            <div class="date-text">
                                <h3>10/9/2026</h3>
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
    background-color: #ffffffca;

    .title {
        justify-items: center;
        align-items: center;

        h1 {
            font-size: 80px;
            font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            color: #222267;
        }
        

    }

    .items {
        display: grid;
        grid-template-columns: auto auto auto;

        .card-space {
            width: 500px;
            height: 550px;
            place-content: center;
            display: flex;

            .card {
                width: 350px;
                height: 400px;
                display: flex;
                flex-direction: column;
                place-items: center;
                background-color: #f5f5f5;
                border-radius: 20px;
                box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 15px 0px;
                padding: 25px;
                font-family: Arial, Helvetica, sans-serif;

                h3 {
                    top: 0;
                    left: 0;
                }


                .image-wrap {
                    width: 300px;
                    height: 200px;
                    align-items: center;
                    display: flex;
                }

                img {
                    width: 300px;
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
        background-color: #ffffffca;

        .title {
            justify-items: center;
            align-items: center;

            h1 {
                font-size: 60px;
                font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
                color: #222267;
            }

        }

        .items {
            display: grid;
            grid-template-columns: auto auto;

            .card-space {
                width: 300px;
                height: 550px;
                place-content: center;
                display: flex;

                .card {
                    width: 200px;
                    height: 400px;
                    display: flex;
                    flex-direction: column;
                    place-items: center;
                    background-color: #f5f5f5;
                    border-radius: 20px;
                    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 15px 0px;
                    padding: 25px;
                    font-family: Arial, Helvetica, sans-serif;

                    h3 {
                        top: 0;
                        left: 0;
                    }

                    .image-wrap {
                        width: 200px;
                        height: 200px;
                        align-items: center;
                        display: flex;
                    }

                    img {
                        width: 200px;
                    }
                }
            }
        }
    }
}
</style>