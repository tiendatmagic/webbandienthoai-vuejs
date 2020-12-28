<template>
  <div id="menu">
    <nav>
      <div id="menu">
        <ul class="root">
    
            <li v-for="menus in menu" v-bind:key="menus">
              <a href="#">  {{ menus}} </a>
            </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
    data() {
        return {
            menu: [
                "Trang chủ",
                "Sản phẩm",
                "Liên hệ"
            ]
        }
    }
};
</script>

<style scoped>
* {
  margin: 0px;
  padding: 0px;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 16px;
}

#menu {
  width: 100%;
  height: 40px;
  background: hotpink;
  margin: 0px auto;
}

ul.root > li {
  list-style: none;
  float: left;
}

ul.root > li > a {
  text-decoration: none;
  padding: 0px 15px 0px 15px;
  line-height: 40px;
  display: block;
  color: #fff;
}


</style>
