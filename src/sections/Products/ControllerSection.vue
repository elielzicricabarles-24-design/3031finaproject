<template>
    <div id="controllers">
        <section class="controllers">
            <div class="container">
                <div class="title">
                    <h1>Controllers</h1>
                    <h2>Integrated software instruments, midi controllers and powerful sequencers</h2>
                </div>
                <div class="items">
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\beatstep_pro.avif" alt="atrolab37"></div>
                            <h2>Beatstep Pro</h2>
                            <p>The ultimate sequencing powerhouse</p>
                        </div>
                    </div>
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\beatstep.avif" alt="atrolab37"></div>
                            <h2>Beatstep</h2>
                            <p>Compact Control Powerhouse</p>
                        </div>
                    </div>
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\beatstep_pro.avif" alt="atrolab37"></div>
                            <h2>Beatstep Pro</h2>
                            <p>The ultimate sequencing powerhouse</p>
                        </div>
                    </div>

                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\keylab_49_mk3.avif" alt="atrolab37"></div>
                            <h2>Keylab 49</h2>
                            <p>Universal MIDI Controller</p>
                        </div>
                    </div>
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\keylab_61_mk3.avif" alt="atrolab37"></div>
                            <h2>Keylab 61</h2>
                            <p>Universal MIDI Controller</p>
                        </div>
                    </div>
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\keylab_88_mk3.avif" alt="atrolab37"></div>
                            <h2>Keylab 88</h2>
                            <p>Universal MIDI Controller</p>
                        </div>
                    </div>

                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\keystep_37_mk2.avif" alt="atrolab37"></div>
                            <h2>Keystep 37 mk2</h2>
                            <p>Controller & Sequencer</p>
                        </div>
                    </div>
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\keystep_pro.avif" alt="atrolab37"></div>
                            <h2>Keystep Pro</h2>
                            <p>Polyphonic sequencing controller keyboard</p>
                        </div>
                    </div>
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\keystep_pro_chroma.avif" alt="atrolab37"></div>
                            <h2>Keystep Pro Chroma</h2>
                            <p>Sequencing mastermind recolored</p>
                        </div>
                    </div>
                    
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\minilab_37.avif" alt="atrolab37"></div>
                            <h2>Minilab 37</h2>
                            <p>Universal music-making controller</p>
                        </div>
                    </div>
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\minilab_3.avif" alt="atrolab37"></div>
                            <h2>Minilab 3</h2>
                            <p>Universal MIDI controller</p>
                        </div>
                    </div>
                    <!--ITEM---->
                    <div class="card-space">
                        <div class="card">
                            <div class="image-wrap"><img src="@\assets\img\product\controllers\microlab_mk3.avif" alt="atrolab37"></div>
                            <h2>Microlab mk3</h2>
                            <p>Universal MIDI controller</p>
                        </div>
                    </div>
                    
                    
                </div>
            </div>
        </section>
    </div>
</template>

<style scoped>
.container{
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-items: center;
    align-items: center;
    background: radial-gradient(circle,rgba(230, 253, 255, 1) 0%, rgba(245, 245, 245, 1) 25%, rgba(245, 245, 245, 1) 43%, rgba(217, 253, 255, 1) 55%, rgba(240, 251, 255, 1) 77%, rgba(227, 249, 255, 1) 100%);


    .title{
        justify-items: center;
        align-items: center;
        text-align: center;
        line-height: 20px;
        padding-bottom: 50px;

        h1{
            font-size: 80px;
            font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
            color: #222267;
        }

        h2{
            font-size: 30px;
            line-height: 30px;
            font-family: Arial, Helvetica, sans-serif;
            color: #3b3bba;
        }
    }

    .items{
        display: grid;
        grid-template-columns: auto auto auto;

        .card-space{
            width: 500px;
            height: 550px;
            place-content: center;
            display: flex;
        

            .card{
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
            line-height: 10px;

            div.card:hover{
                width: 360px;
                height: 410px;
                box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 15px 10px;
            }

            .image-wrap{
                width: 300px;
                height: 250px;
                align-items: center;
                place-content: center;
                display: flex;
            }

            img{
                width: 300px;
                place-items: center;
                transition: width 0.25s;
                transition-timing-function: cubic-bezier(0.42, 0, 0.31, 1.03);
            }

            img:hover{
                width: 320px;
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
                    height: 350px;
                    display: flex;
                    flex-direction: column;
                    place-items: center;
                    background-color: #f5f5f5;
                    border-radius: 20px;
                    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 15px 0px;
                    padding: 25px;
                    font-family: Arial, Helvetica, sans-serif;
                    line-height: 30px;

                    h3 {
                        top: 0;
                        left: 0;
                    }

                    h2{
                        font-size: 20px;
                    }

                    .image-wrap {
                        width: 200px;
                        height: 150px;
                        align-items: center;
                        display: flex;
                    }

                    img {
                        width: 200px;
                    }

                        img:hover {
                        width: 220px;
                    }
                }
            }
        }
    }
}

</style> 