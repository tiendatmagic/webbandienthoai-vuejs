<template>
  <div id="list-card">
    <div class="card" v-for="cards in card" v-bind:key="cards">
      <img :src="cards.img" />
      <div class="card-body">
        <a href="###"
          ><h5 class="card-title">{{ cards.name }}</h5></a
        >
        <div class="card-text">
          <b>Giá: </b><span class="money">{{ cards.money }} đ</span>
        </div>
        <div class="btn-group">
          <button class="btn-cart">Thêm vào giỏ hàng</button
          ><button class="btn-buy">Mua ngay</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      card: [
        {
          img:
            "https://cdn.tgdd.vn/Products/Images/42/220438/TimerThumb/OPPO-Reno5-trang-600x600.jpg",
          name: "Oppo reno5",
          money: 8990000,
        },

        {
          img:
            "https://cdn.tgdd.vn/Products/Images/42/228736/iphone-12-trang-new-600x600-600x600.jpg",
          name: "iPhone12 128GB",
          money: 24990000,
        },

        {
          img:
            "https://cdn.tgdd.vn/Products/Images/42/205773/samsung-galaxy-a10s-xanh-600x600.jpg",
          name: "Samsung Galaxy A10s",
          money: 2490000,
        },

        {
          img:
            "https://cdn.tgdd.vn/Products/Images/42/228453/TimerThumb/vivo-v20-(4).jpg",
          name: "Vivo V20",
          money: 7990000,
        },

        {
          img:
            "https://cdn.tgdd.vn/Products/Images/42/214924/TimerThumb/xiaomi-redmi-note-9s-(37).jpg",
          name: "Xiaomi redmi note 9S",
          money: 5690000,
        },
      ],
    };
  },
  methods: {
    abc: function () {
      alert(this.card[1].name1);
    },
  },
};
</script>

<style scoped>
* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

#list-card {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
}
.card {
  width: 270px;
  text-align: center;
  border: 0.1px solid #c2c2c2;
  font-family: Arial, Helvetica, sans-serif;
  border-radius: 9px;
  overflow: hidden;
  cursor: pointer;
  transition: 0.2s ease-out;
}
.card:hover {
  box-shadow: 4px 4px 5px 0px rgba(0, 0, 0, 0.25);
  transition: 0.2s ease-out;
}
.card img {
  width: 100%;
  height: 270px;
}
.card-body a {
  text-decoration: none;
}
.card-title {
  color: #1495ff;
  text-transform: uppercase;
  font-size: 22px;
  margin-top: 10px;
}
.card-text {
  margin-top: 10px;
  font-size: 18px;
}
.btn-group {
  display: flex;
  justify-content: space-evenly;
  margin-top: 15px;
  margin-bottom: 15px;
}
.btn-group button {
  color: #fff;
  border-color: #dc3545;
  display: inline-block;
  font-weight: 400;
  text-align: center;
  border: 1px solid transparent;
  outline: none;
  padding: 0.375rem 0.75rem;
  font-size: 1rem;
  line-height: 1.5;
  border-radius: 0.25rem;
  cursor: pointer;
}
.btn-group button:hover {
  filter: brightness(90%);
}
.btn-group .btn-cart {
  background-color: #dc3545;
}
.btn-group .btn-buy {
  background-color: #7fc400;
}
</style>
