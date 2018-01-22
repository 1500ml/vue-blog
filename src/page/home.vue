<template>
  <div>
    <Header></Header>
    <div class="jztop"></div>
<div class="container">

  <div class="bloglist f_l">
    <div  class=" right_of_menu">
    <h3><a href="#">【心路历程】今天开始，我打算做点什么属于自己的东西了</a></h3>
    <figure><img src="../../static/images/img_1.jpg"></figure>
    <ul>
      <p> 前行吧。</p>
      <a title="" class="readmore" href="#" target="_blank">阅读全文&gt;&gt;</a>
    </ul>
    <p class="dateview"><span>2017-07-13</span><span>作者：</span><span>个人博客：[<a href="">心得笔记</a>]</span></p>
    </div>
  </div>

  <div class="r_box f_r">
    <div class="tit01">
      <h3 class="tit">我</h3>
      <div class="gzwm">
        <ul>
          <li><a class="email" href="#" target="_blank">我的电话</a></li>
          <li><a class="qq" href="#" target="_blank">我的邮箱</a></li>
          <li><a class="tel" href="#" target="_blank">我的QQ</a></li>
          <li><a class="prize" href="#">我的微博</a></li>
        </ul>
      </div>
    </div>
  </div>

</div>

    <div class="jzend"></div>
    <Footer></Footer>
  </div>
</template>
<script>
  import Header from '../components/header.vue'
  import Footer from '../components/footer.vue'

  export  default {
    components: { Header, Footer },
    data () {
      return {
        list: []
      }
    },

    created(){

    },
    methods:{

      }
  }
</script>

<style>
  @import "../../static/css/base.css";
  @import "../../static/css/index.css";
  @import "../../static/css/main.css";
</style>
