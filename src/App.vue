<template>
  <div class="statusbar"></div>
  <div class="panel panel-left panel-cover sidebar-left">
    <div class="page">
      <div class="page-content">
        <div class="user-view">
          <div class="background-view">
            <img src="/images/bg-user.jpg" alt="">
          </div>
          <img class="circle responsive-img" src="/images/profile.png" alt="">
          <span class="white-text name">Hasin Hayder</span>
        </div>
        <div class="list links-list">
          <ul>
            <li>
              <a href="/product/" class="panel-close"><i class="fa fa-support"></i>Product</a>
            </li>
<!--            <li>-->
<!--              <a href="/product-details/" class="panel-close"><i class="fa fa-clone"></i>Product Details</a>-->
<!--            </li>-->
<!--            <li>-->
<!--              <a href="/wishlist/" class="panel-close"><i class="fa fa-bookmark"></i>Wishlist</a>-->
<!--            </li>-->
<!--            <li>-->
<!--              <a href="/cart/" class="panel-close"><i class="fa fa-shopping-cart"></i>Cart</a>-->
<!--            </li>-->
<!--            <li>-->
<!--              <a href="/checkout/" class="panel-close"><i class="fa fa-send"></i>Checkout</a>-->
<!--            </li>-->
<!--            <li>-->
<!--              <a href="/blog/" class="panel-close"><i class="fa fa-file-o"></i>Blog</a>-->
<!--            </li>-->
<!--            <li>-->
<!--              <a href="/about/" class="panel-close"><i class="fa fa-user"></i>About</a>-->
<!--            </li>-->
<!--            <li>-->
<!--              <a href="/contact/" class="panel-close"><i class="fa fa-envelope"></i>Contact</a>-->
<!--            </li>-->
<!--            <li>-->
<!--              <a href="/login/" class="panel-close"><i class="fa fa-sign-in"></i>Login</a>-->
<!--            </li>-->
<!--            <li>-->
<!--              <a href="/register/" class="panel-close"><i class="fa fa-user-plus"></i>Register</a>-->
<!--            </li>-->
          </ul>
        </div>
      </div>
    </div>
  </div>
  <div class="view view-main view-init ios-edges" data-url="/">
    <div class="page">

      <!-- navbar -->
      <div class="navbar navbar-cart">
        <div class="navbar-inner">
          <div class="left">
            <a href="#" class="link icon-only panel-open" data-panel="left">
              <i class="fa fa-bars"></i>
            </a>
          </div>
          <div class="title sliding title-heading"><a href="/home/"><h1>Landing Page</h1></a></div>
          <div class="right icon-cart">
            <a class="link icon-only searchbar-enable" href="/cart/">
              <i class="fa fa-shopping-cart"></i>
              <sup>3</sup>
            </a>
          </div>
        </div>
      </div>
      <!-- end navbar -->

      <div class="page-content">

        <!-- slide-shop -->
<!--        <div class="slide-shop">-->
<!--          <div data-pagination='{"el": ".swiper-pagination", "hideOnClick": true}' class="swiper-container swiper-init demo-swiper">-->
<!--            <div class="swiper-pagination"></div>-->
<!--            <div class="swiper-wrapper">-->
<!--              <div class="swiper-slide">-->
<!--                <div class="slide-content">-->
<!--                  <div class="mask"></div>-->
<!--                  <img src="/images/slider1.jpg" alt="">-->
<!--                  <div class="intro-caption">-->
<!--                    <h2>eCommerce Landing Page</h2>-->
<!--                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat, quos?</p>-->
<!--                    <button class="button">Shop Now</button>-->
<!--                  </div>-->
<!--                </div>-->
<!--              </div>-->
<!--              <div class="swiper-slide">-->
<!--                <div class="slide-content">-->
<!--                  <div class="mask"></div>-->
<!--                  <img src="/images/slider2.jpg" alt="">-->
<!--                  <div class="intro-caption">-->
<!--                    <h2>Happy Shopping Now</h2>-->
<!--                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat, quos?</p>-->
<!--                    <button class="button">Shop Now</button>-->
<!--                  </div>-->
<!--                </div>-->
<!--              </div>-->
<!--              <div class="swiper-slide">-->
<!--                <div class="slide-content">-->
<!--                  <div class="mask"></div>-->
<!--                  <img src="/images/slider3.jpg" alt="">-->
<!--                  <div class="intro-caption">-->
<!--                    <h2>Get Discount 50% Off</h2>-->
<!--                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Repellat, quos?</p>-->
<!--                    <button class="button">Shop Now</button>-->
<!--                  </div>-->
<!--                </div>-->
<!--              </div>-->
<!--            </div>-->
<!--          </div>-->
<!--        </div>-->
        <!-- end slide shop-->

        <!-- category -->
        <div class="category segments-top">
          <div class="container">
            <div class="section-title">
              <h3>Category</h3>
            </div>
            <div class="row">
              <div class="col">
                <a href="">
                  <div class="content">
                    <i class="fa fa-female"></i>
                    <span>Fashion</span>
                  </div>
                </a>
              </div>
              <div class="col">
                <a href="">
                  <div class="content">
                    <i class="fa fa-child"></i>
                    <span>Kidz</span>
                  </div>
                </a>
              </div>
              <div class="col">
                <a href="">
                  <div class="content">
                    <i class="fa fa-camera"></i>
                    <span>Camera</span>
                  </div>
                </a>
              </div>
            </div>
            <div class="row">
              <div class="col">
                <a href="">
                  <div class="content">
                    <i class="fa fa-globe"></i>
                    <span>Digital</span>
                  </div>
                </a>
              </div>
              <div class="col">
                <a href="">
                  <div class="content">
                    <i class="fa fa-support"></i>
                    <span>Sport</span>
                  </div>
                </a>
              </div>
              <div class="col">
                <a href="">
                  <div class="content">
                    <i class="fa fa-mobile"></i>
                    <span>Smartphone</span>
                  </div>
                </a>
              </div>
            </div>
          </div>
        </div>
        <!-- end category -->

        <!-- product home -->
        <div class="product product-home popular-product segments">
          <div class="container">
            <div class="section-title">
              <h3>Popular Product</h3>
            </div>
            <div class="row">

              <div class="col" v-for="item in popularProducts" :key="item.id">
                <div class="conent">
                  <img :src="item.thumbnail" alt="" >
                  <a href="#"><p>{{ item.title }}</p></a>
                  <h5>{{ item.price }}</h5>
                </div>
              </div>
            </div>
            <div class="row">

              <div class="col" v-for="item in popularProduct2s" :key="item.id">
                <div class="conent">
                  <img :src="item.thumbnail" alt="">
                  <a href="#"><p>{{ item.title }}</p></a>
                  <h5>{{ item.price }}</h5>
                </div>
              </div>

            </div>
          </div>
        </div>
        <!-- end product home -->

        <!-- product home -->
        <div class="product product-home new-product segments-bottom">
          <div class="container">
            <div class="section-title">
              <h3>New Product</h3>
              <div class="wrap-more">
                <a href="">See More <i class="fa fa-angle-right"></i></a>
              </div>
            </div>
            <div class="row">
              <div class="col s6" v-for="item in newProducts" :key="item.id">
                <div class="conent">
                  <img :src="item.thumbnail" alt="">
                  <a href="#"><p>{{ item.title }}</p></a>
                  <h5>{{ item.price }}</h5>
                </div>
              </div>
            </div>

            <div class="row">
              <div class="col s6" v-for="item in newProduct2s" :key="item.id">
                <div class="conent">
                  <img :src="item.thumbnail" alt="">
                  <a href="#"><p>{{ item.title }}</p></a>
                  <h5>{{ item.price }}</h5>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- end product home -->

        <!-- footer -->
        <footer class="segments">
          <div class="container">
            <h1>Landing Page</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit Ipsam voluptate laborum harum nam ratione.</p>
            <ul>
              <li><a href=""><i class="fa fa-facebook"></i></a></li>
              <li><a href=""><i class="fa fa-twitter"></i></a></li>
              <li><a href=""><i class="fa fa-google"></i></a></li>
              <li><a href=""><i class="fa fa-instagram"></i></a></li>
            </ul>
            <p>Copyright © All Right Reserved</p>
          </div>
        </footer>
        <!-- end footer -->

      </div>
    </div>
  </div>
</template>

<script setup>

const popularProducts = [
  {
    id:1,
    title:"Fashion for Man Modern Style",
    thumbnail:"/images/product1.png",
    price:"$28",
  },
  {
    id:2,
    title:"Trendy Fashion for Man Modern Style",
    thumbnail:"/images/product5.png",
    price:"$11",
  },
];

const popularProduct2s = [
  {
    id:1,
    title:"Fashion for Man Modern Style Dark",
    thumbnail:"/images/product3.png",
    price:"$32",
  },
  {
    id:2,
    title:"Casual SFashion for Man Modern Style",
    thumbnail:"/images/product4.png",
    price:"$23",
  },
];

const newProducts = [
  {
    id:1,
    title:"Fashion for Man Modern Style",
    thumbnail:"/images/product5.png",
    price:"$28",
  },
  {
    id:2,
    title:"Fashion for Man Modern Style",
    thumbnail:"/images/product7.png",
    price:"$22",
  },

];

const newProduct2s = [

  {
    id:3,
    title:"Fashion for Man Modern Style Dark",
    thumbnail:"/images/product6.png",
    price:"$33",
  },
  {
    id:4,
    title:"Fashion for Man Modern Style Comfortable",
    thumbnail:"/images/product8.png",
    price:"$25",
  },

];

</script>

<style>

</style>
