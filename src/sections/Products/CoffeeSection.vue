<template>
  <div id="coffee">
    <section class="coffee">
      <div class="container">
        <div class="title">
          <h1>Coffee</h1>
          <h2>Choose your favorite drink</h2>
        </div>
        <div class="drinks">
          <div class="card-space">
            <div class="card">
              <div class="image-wrap">
                <img src="@\assets\img\product\coffee\caramel_macchiato.png" alt="Caramel Macchiato" />
              </div>
              <h2>Caramel Macchiato</h2>
              <p>A smooth coffee with caramel sweetness</p>
              <p>₱37 (add ₱15 for upsize)</p>
            </div>
          </div>

          <div class="card-space">
            <div class="card">
              <div class="image-wrap">
                <img src="@\assets\img\product\coffee\creamy_latte.png" alt="Creamy Latte" />
              </div>
              <h2>Creamy Latte</h2>
              <p>A creamy, comforting coffeee drink</p>
              <p>₱37 (add ₱15 for upsize)</p>
            </div>
          </div>

          <div class="card-space">
            <div class="card">
              <div class="image-wrap">
                <img src="@\assets\img\product\coffee\french_vanilla.png" alt="French Vanilla" />
              </div>
              <h2>French Vanilla</h2>
              <p>Coffee with a smooth vanilla flavor</p>
              <p>₱37 (add ₱15 for upsize)</p>
            </div>
          </div>

          <div class="card-space">
            <div class="card">
              <div class="image-wrap">
                <img src="@\assets\img\product\coffee\spanish_latte.png" alt="Spanish Latte" />
              </div>
              <h2>Spanish Latte</h2>
              <p>A rich latte with a touch of sweetness</p>
              <p>₱37 (add ₱15 for upsize)</p>
            </div>
          </div>

          <div class="card-space">
            <div class="card">
              <div class="image-wrap">
                <img src="@\assets\img\product\coffee\vietnamese_latte.png" alt="Vietnamese Latte" />
              </div>
              <h2>Vietnamese Latte</h2>
              <p>A bold coffee with a creamy finish</p>
              <p>₱37 (add ₱15 for upsize)</p>
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
  align-items: center;
  background: linear-gradient(360deg, #fafafa 0%, #7ac250 50%, #60dd18 100%);
  padding-bottom: 50px;
  padding-top: 100px;

  .title {
    justify-items: center;
    align-items: center;
    text-align: center;
    line-height: 20px;

    h1 {
      font-size: 85px;
      font-family: Verdana, Geneva, Tahoma, sans-serif;
      color: #ffffff;
    }

    h2 {
      font-size: 30px;
      line-height: 30px;
      font-family: Verdana, Geneva, Tahoma, sans-serif;
      color: #055309;
    }
  }

  .drinks {
    display: grid;
    grid-template-columns: 450px 450px 500px;

    .card-space {
      width: 500px;
      height: 500px;
      place-content: center;
      display: flex;

      .card {
        width: 350px;
        height: 400px;
        display: flex;
        flex-direction: column;
        place-items: center;
        background-color: rgba(255, 255, 255, 0.85);
        border-radius: 15px;
        padding: 10px;
        font-family: Arial, Helvetica, sans-serif;
        line-height: 10px;

        .image-wrap {
          width: 300px;
          height: 250px;
          align-items: center;
          place-content: center;
          display: flex;
        }

        img {
          width: 180px;
          height: 250px;
          place-items: center;
          transition:
            width 0.2s,
            height 0.2s;
        }

        img:hover {
          width: 200px;
          height: 270px;
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
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        color: #fafafa;
      }
    }

    .drinks {
      display: grid;
      grid-template-columns: 1fr;
      gap: 60px;

      .card-space {
        width: 100%;
        height: 100%;

        .card {
          width: 250px;
          height: 100%;
          display: flex;
          flex-direction: column;
          place-items: center;
          background-color: #f5f5f5;
          border-radius: 20px;
          padding: 25px;
          font-family: Arial, Helvetica, sans-serif;
          line-height: 30px;

          h2 {
            font-size: 25px;
          }

          .image-wrap {
            width: 200px;
            height: 150px;
            align-items: center;
            display: flex;
          }

          img {
            width: 130px;
            height: 180px;
            transition: width 0.2s;
          }

          img:hover {
            width: 150px;
            height: 160px;
          }
        }
      }
    }
  }
}
</style>
