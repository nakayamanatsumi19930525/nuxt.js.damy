<template>
  <div>
    <nav class="navbar navbar-expand-lg  fixed-top" style="background-color: #FEFFD3;" id="mainNav">
      <div class="container">
       <a class="navbar-brand" href="/">
        <img src="~assets/images/00022.png" class="logo" alt="">
        </a> 
        <div class="pc-only01">
              <p class="logo-des">いいいいではたらく<br>
                おおおおおおおサービス</p>
              <div class="collapse navbar-collapse" id="navbarResponsive">
                <ul class="navbar-nav ml-auto">
                  <li class="nav-item">
                    <router-link class="nav-link download" to="/">資料ダウンロード</router-link>
                  </li>
                  <li class="nav-item">
                    <router-link class="nav-link individual" to="/about">〇〇様へ</router-link>
                  </li>
                  <li class="nav-item contact-item">
                    <a class="nav-link contact-btn" href="/Contact">お問い合わせ</a>
                  </li>
                </ul>
              </div>
         </div>
      </div>
    </nav>
  <nuxt />
  

    <footer>
      <div class="container">
        <div class="row">
          <div class="col-lg-8 col-md-10 mx-auto text-center footer-sec">
            <p>あああああああああああああああああああああああああああああああああああああ</p>
             <a class="navbar-brand" href="/">
        <img src="~assets/images/00022.png" class="footer-logo" alt="">
        </a> 
            <a class="nav-link footer-contact-btn mx-auto" href="/post">お問い合わせ</a>
            <p class="footer-address text-center">〒111-1111 東京都ああああああああああああああああああああああああああああああ</p>
            <p class="copyright text-center">&copy;TSUTSUMU Inc.</p>
          </div>
        </div>
      </div>
    </footer>

  </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>

$sp:375px;
 
@mixin sp {
  @media screen and (max-width: ($sp)) {
    @content;
  }
}


#mainNav{
  height: 100px;
}

a.nuxt-link-exact-active{
    font-weight: bold;
  }

.logo{
  width: 318px;
}

.pc-only01{
  display: flex;
}

.logo-des{
  font-size: 13px;
  line-height: 18px;
  font-weight: bold;
  background-color: #fff;
  width: 195px;
  height: 55px;
  margin: 0 100px 0 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

.download{
  position: relative;
}

.download::after{
  content: "";
  display: inline-block;
  width: 25px;
  height: 25px;
  background: url(~assets/images/header001.png) no-repeat;
  background-size: contain;
  margin-right: 8px;
  transform: translate(20%,20%)
}

.individual{
  position: relative;
}

.individual::after{
  content: "";
  display: inline-block;
  width: 25px;
  height: 25px;
  background: url(~assets/images/header002.png) no-repeat;
  background-size: contain;
  margin-right: 8px;
  transform: translate(20%,20%)
}


.contact-btn{
  background: #fff;
  border-radius: 60px;
  padding: 10px 30px;
  width: 148px;
 text-align: center;
}

.nav-item{
  margin-right: 10px;
}

footer{
    background-color: lightcoral;
}


 .footer-contact-btn{
  background: #fff;
  border-radius: 10px;
  line-height: 58px;
  width: 227px;
  font-size: 20px;
  font-weight: bold;
  margin-bottom: 40px;
 /* padding: 10px 30px; */
}

 .footer-address , .copyright{
   color: #fff;
  }

.footer-logo{
  width: 137px;
  height: 50px;
  margin-bottom: 22px;
margin-top: 20px;
}

.footer-sec{
   margin-top: 40px;
}


/* ----------------------------- */
.navbar-brand{
    @include sp{
    margin: 0 auto;
  }
}


.navbar-brand img{
  @include sp{
    width: 200px;
  }

}

.pc-only01{
    @include sp{
    display: none;
  }
}


#mainNav{
  @include sp{
    width:375px;
  }
}
</style>



