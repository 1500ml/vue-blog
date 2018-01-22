<template>
  <header>
    <div class="topnav"></div>
    <div id="warapper">
      <div class="headtop"></div>
      <div class="contenttop">
        <div class="logo f_l">一只很怂很怂的代码猴子</div>
        <div class="search f_r">
          <input name="keyboard" id="keyboard" class="input_text" :placeholder="holder"/>
          <button v-text="btnText" class="input_submit" @click="search"></button>
        </div>
        <div class="blank"></div>
        <nav>
          <div class="navigation">
            <ul class="menu">
              <li v-for="item in MenuItems">
                <router-link :to="item.href">
                  {{ item.message }}
                </router-link>
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
  import Vue from 'vue'

  export default {
    data: function () {
      return {
        holder: '请输入搜索信息',
        btnText: "搜索",
        MenuItems: [
          {message: '网站首页', href: '#'},
          {message: '关于我', href: ''},
          {message: '点点滴滴', href: ''},
          {message: '留言板', href: ''},
          {message: '联系我', href: ''}
        ]
      }
    },
    methods: {
      search: function () {
        console.log(this.holder)
      }
    }
  }
</script>


<style scoped>
  @import "../../static/css/index.css";
  @import "../../static/css/main.css";

  body {
    font: 12px "宋体", Arial, Helvetica, sans-serif;
    color: #666666;
    background: url(../../static/images/bg.jpg) repeat
  }

</style>
