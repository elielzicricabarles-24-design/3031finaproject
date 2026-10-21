<template>
    <div id="ContactSection">
        <section class="Contacts">
            <div class="container">
                <div class="title">
                    <h1>Contact Us</h1>
                    <h2>Reach us through any of these</h2>
                </div>
                <div class="items">
                    <div class="card-space">
                        <div class="card">
                            <div class="icon-wrap"><img src="@/assets/img/contact/Facebook.png" alt="Facebook"></div>
                            <h3>Facebook</h3>
                            <p>Panda Coffee</p>
                        </div>
                    </div>

                    <div class="card-space">
                        <div class="card">
                            <div class="icon-wrap"><img src="@/assets/img/contact/Gmail.png" alt="Gmail"></div>
                            <h3>Gmail</h3>
                            <p>pandacoffee@gmail.com</p>
                        </div>
                    </div>

                    <div class="card-space">
                        <div class="card">
                            <div class="icon-wrap"><img src="@/assets/img/contact/Contact.png" alt="Contact"></div>
                            <h3>Contact</h3>
                            <p>0948-048-1581</p>
                        </div>
                    </div>

                </div>
            </div>
        </section>
    </div>
</template>

<style scoped>
.container {
    overflow-x: hidden;
    width: 100%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 50px;
    padding-bottom: 50px;
    background-color: rgb(136, 218, 92);
    background-image: url('@/assets/img/background/green_bubble_bg.png');
    background-position: 0px -200px;

    .title {
        text-align: center;
        line-height: 20px;
        padding-bottom: 50px;

        h1 {
            font-size: 60px;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            color: #fafffb;
        }

        h2 {
            font-size: 24px;
            line-height: 30px;
            font-family: Arial, Helvetica, sans-serif;
            color: #328a1c;
        }
    }

    .items {
        display: grid;
        grid-template-columns: auto auto auto;
        justify-content: center;
        gap: 30px;

        .card-space {
            display: flex;
            place-content: center;

            .card {
                width: 300px;
                height: 300px;
                display: flex;
                flex-direction: column;
                place-items: center;
                place-content: center;
                background-color: #f5f5f5;
                border-radius: 20px;
                box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 15px 0px;
                padding: 25px;
                font-family: Arial, Helvetica, sans-serif;
                text-align: center;

                .icon-wrap {
                    width: 120px;
                    height: 120px;
                    display: flex;
                    align-items: center;
                    place-content: center;
                }

                img {
                    width: 100%;
                    transition: transform 0.25s;
                    transition-timing-function: cubic-bezier(0.42, 0, 0.31, 1.03);
                }

                img:hover {
                    transform: scale(1.2);
                    /* icon grows on hover */
                }

                h3 {
                    font-size: 24px;
                    color: #672222;
                    margin: 20px 0 5px;
                }

                p {
                    font-size: 16px;
                    color: #ba3b3b;
                    margin: 0;
                }
            }
        }
    }
}

@media (max-width: 900px) {
    .container {
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-top: 50px;
        padding-bottom: 50px;
        background-color: rgb(136, 218, 92);
        background-image: url('@/assets/img/background/green_bubble_bg.png');
        background-position: 0px 0px;
        padding-top: 150px;

        .title {
            text-align: center;
            line-height: 20px;
            padding-bottom: 50px;

            h1 {
                font-size: 60px;
            }

            h2 {
                font-size: 24px;
                line-height: 30px;
            }
        }

        .items {
            display: grid;
            grid-template-columns: auto auto;
            justify-content: center;
            gap: 30px;

            .card-space {
                display: flex;
                place-content: center;

                .card {
                    width: 200px;
                    height: 200px;
                    display: flex;
                    flex-direction: column;
                    place-items: center;
                    place-content: center;
                    background-color: #f5f5f5;
                    border-radius: 20px;
                    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 15px 0px;
                    padding: 25px;
                    font-family: Arial, Helvetica, sans-serif;
                    text-align: center;

                    .icon-wrap {
                        width: 100px;
                        height: 100px;
                        display: flex;
                        align-items: center;
                        place-content: center;
                    }

                    img {
                        width: 100%;
                        transition: transform 0.25s;
                        transition-timing-function: cubic-bezier(0.42, 0, 0.31, 1.03);
                    }

                    img:hover {
                        transform: scale(1.2);
                        /* icon grows on hover */
                    }

                    h3 {
                        font-size: 20px;
                        color: #222267;
                        margin: 20px 0 5px;
                    }

                    p {
                        font-size: 16px;
                        margin: 0;
                    }
                }
            }
        }
    }
}
</style>