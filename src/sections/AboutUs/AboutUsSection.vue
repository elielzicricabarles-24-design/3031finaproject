<template>
  <div class="about-us">
    <section class="about-us">
      <div class="container">
        <div class="left-content">
          <div class="title">
            <h1>About Us</h1>
          </div>
          <div class="about-text">
            <div class="about-text-column">
              <h2>Good Coffee, Everyday Prices</h2>
              <p>
                Panda Coffee Ph serves great drinks that anyone can enjoy. We believe good coffee
                should not be expensive.
              </p>
            </div>

            <div class="about-text-column">
              <h2>The Perfect Mix</h2>
              <p>
                We are your one-stop drink shop. Enjoy our smooth Caramel Macchiatos, bright Matcha,
                or sweet Choco Wacko.
              </p>
            </div>

            <div class="about-text-column">
              <h2>Made for You</h2>
              <p>
                We love being your friendly neighborhood spot. Whether you are a student on the go
                or just catching up with friends, we welcome you with great drinks and a warm smile.
              </p>
            </div>
          </div>
        </div>

        <div class="right-img">
          <img src="@/assets/img/graphic/icon.png" alt="Logo" />
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
.container {
  overflow-x: hidden;
  height: 100vh;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  background-color: rgb(136, 218, 92);
  background-image: url('@/assets/img/background/green_bubble_bg.png');

  .left-content {
    width: 60%;
  }

  .title {
    display: flex;
    justify-items: center;
    align-items: center;
    padding: 10px 20px;

    h1 {
      height: 2vh;
      font-size: 76px;
      line-height: 50px;
      font-family: Verdana, Geneva, Tahoma, sans-serif;
      color: #f8f8f9;
    }
  }

  .about-text {
    width: auto;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
    column-gap: 40px;
    padding: 0 35px;

    .about-text-column p {
      font-size: 20px;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      padding: 0;
    }

    .about-text-column h2 {
      height: 8vh;
      font-size: 25px;
      font-family: Verdana, Geneva, Tahoma, sans-serif;
      color: #124716;
    }
  }

  .right-img {
    display: flex;
    justify-content: center;
    padding: 0 50px;

    img {
      width: 300px;
      height: 300px;
    }
  }
}

@media (max-width: 768px) {
  .container {
    width: 100%;
    height: auto;
    flex-direction: column;
    align-items: stretch;
    padding-top: 100px;

    .left-content {
      width: 100%;
    }

    .title {
      padding: 24px 0px;

      h1 {
        height: auto;
        font-size: 48px;
        line-height: 1.1;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        color: #f8f8f9;
      }
    }

    .about-text {
      width: 100%;
      height: auto;
      grid-template-columns: 1fr;
      gap: 20px;
      padding: 0 0px 24px;

      .about-text-column h2 {
        width: 80%;
        height: auto;
        margin: 0 0 8px;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-size: 20px;
      }

      .about-text-column p {
        font-size: 16px;
        line-height: 1.5;
        margin: 0;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      }
    }

    .right-img {
      padding: 0 20px 24px;

      img {
        width: 300px;
        height: 300px;
      }
    }
  }
}
</style>
