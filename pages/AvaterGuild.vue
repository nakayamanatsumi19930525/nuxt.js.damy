<template>
  <div id="container2">
    <h2>あああああああああああ</h2>
    <div class="des">
      あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ。<br>
      あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ。ああああああああああああああああああああああああ
    </div>

    <Title id=avater-title>ああああああああああああああああああ</Title>
    <div class="avater-section">
    <div class="sec2">
      あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ。あああああああああああああああああああ<br>
      あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ。ああああああああああああああああああああああああ
    </div>
    <div class="img">
    <img class="sec2-item-img" src="~assets/images/00026.png" alt="">
    </div>
   </div>
   <div class="sp-only">
     <a class="nav-link contact-btn mx-auto" href="/post">お問い合わせはこちら</a>
   </div>
  </div>
</template>

<script>
import Title from "~/components/Title.vue";
export default {
  components: {
    Title
  }
};
</script>


<style lang="scss" scoped>

$sp:375px;
 
@mixin sp {
  @media screen and (max-width: ($sp)) {
    @content;
  }
}


#container2{
  width: 893px;
  background-color: #FEFFD3;


 > h2{
  color:#ef6687;
  font-size: 45px;
  font-family: Barlow;
  font-weight: bold;
  text-align: center;
  margin-top: 25px;
  }

  > .des{
  margin: 56px auto 66px;
  text-align: center;
  font-size: 23px;
  font-weight: bold;
  line-height: 2;
  width: 692px;
  }
}

#avater-title{
  width: 500px;
  text-align: center;
    position: relative;
}

.avater-section{
  margin-left: -25px;
}

.sec2{
    font-size: 16px;
    text-align: center;
    line-height: 2;
    font-weight: bold;
    width: 893px;
    margin: -20px auto 0;
    padding: 66px 110px 54px 110px;
    background: #fff;
    border-radius: 30px 30px 0 0;
}

.img{
  text-align: center;
  width: 100%;

  > .sec2-item-img{
    width: 893px;
    }

}

.sp-only{
  display: none;
}

/* ----------------------------- */


#container2
  h2{
  @include sp{
   font-size: 22px;
  }
}

#container2 .des{
  @include sp{
    font-size: 16px;
    width: 325px;
  }
}

.sec2{
  @include sp{
    width: 351px;
    padding: 66px 13px 45px 13px;
  }
}

.avater-section{
  @include sp{
    width: 325px;
  }
}

.img {
  > .sec2-item-img{
    @include sp{
      width: 351px;
      border-radius: 0 0 27px 27px;
    }
  }
}

.sp-only{
  @include sp{
    display: inline;
    text-align: center;

  }
}
.contact-btn{
  @include sp{
  width: 349px;
  height: 66px;
  padding: 18px 71px 23px 71px;
  border-radius: 10px;
  border: solid 1px #ef6687;
  background-color: #ffffff;
  font-size: 20px;
  color: #ef6687;
    margin-top: 81px;
  }
}
</style>