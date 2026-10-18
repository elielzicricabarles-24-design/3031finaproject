<template>
  <section class="tea">
    <h1 class="tea_title">Tea</h1>
    <div class="tea_item">
      <h2>Cheesecake Milk Tea Series</h2>
      <div class="price">
        <h3>₱69</h3>
      </div>
      <h4>(22oz only)</h4>

      <img src="@/assets/img/product/tea/cheesecake_tea.jpg" alt="Cheesecake Milk Tea drinks" />

      <div class="flavors">
        <div>
          <p>· Matcha</p>
          <p>· Taro</p>
          <p>· Cookies & Cream</p>
          <p>· Avocado</p>
        </div>

        <div>
          <p>· Brown Sugar</p>
          <p>· Okinawa</p>
          <p>· Hokkaido</p>
          <p>· Wintermelon</p>
        </div>
      </div>
    </div>

    <div class="tea_item">
      <h2>Wintermelon Tea Series</h2>
      <div class="price">
        <h3>₱69</h3>
      </div>
      <h4>(22oz only)</h4>
      <img src="@/assets/img/product/tea/wintermelon_tea.jpg" alt="Wintermelon Tea Series" />

      <div class="flavors">
        <div>
          <p>· Lemon</p>
        </div>
        <div>
          <p>· Passion Fruit</p>
        </div>
      </div>
    </div>

    <div class="tea_item">
      <h2>Milktea</h2>
      <div class="price">
        <h3>₱39/₱49</h3>
      </div>
      <h4></h4>
      <img src="@/assets/img/product/tea/Milktea.jpg" />

      <div class="flavors">
        <div>
          <p>· Okinawa</p>
          <P>· Hokkaido</P>
          <p>· Wintermelon</p>
        </div>
        <div>
          <p>· Cookies and Cream</p>
          <p>· Creamy Avocado</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.tea {
  padding: 40px 30px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 24px;
}

.tea_title {
  width: 100%;
  text-align: center;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-size: 85px;
  color: #055309;
}

.tea_item {
  font-family: Arial, Helvetica, sans-serif;
  width: 100%;
  max-width: 500px;
}

.tea_item h2 {
  text-align: center;
}

.tea_item img {
  width: 100%;
  height: 50vh;
}

.flavors {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
}

.flavors p {
  margin: 6px 0;
  font-size: 20px;
  font-weight: bold;
}

img {
  border-radius: 30px;
}

.tea_item {
  display: flex;
  flex-direction: column;
  justify-items: center;
  align-items: center;
  line-height: 20px;
  padding-bottom: 50px;

  h1 {
    font-size: 80px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    color: #316722;
  }

  h2 {
    font-size: 30px;
    line-height: 30px;
    font-family: Arial, Helvetica, sans-serif;
    color: #3bba6c;
  }

  .price {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 200px;
    height: 50px;
    font-size: 35px;
    font-family: Arial, Helvetica, sans-serif;
    background-color: #22672c;
    color: #f5f5f5;
    border-radius: 30px;
    margin-bottom: 10px;
  }
}


@media (max-width: 768px) {
  .tea {
    flex-direction: column;
    align-items: center;
  }

  .tea-item {
    width: 100%;
    max-width: 500px;
  }

  .tea-title {
    font-size: 60px;
  }

  .tea_item img {
    height: auto;
  }

  .flavors p {
    font-size: 16px;
  }
}
</style>
