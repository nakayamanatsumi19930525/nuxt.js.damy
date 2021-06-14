<template>
<div>
        <div class="bg"> </div>
    <div id="container3">
    <Title id=avater-title>サポート体制</Title>
     <h3>ああああああああああああああああああああああああああああああああ<br>
    あああああああああああああああああああああああああああああ。</h3>
    <div class="support-sec">
    <div class="support-sec-01 sec-02">
      <p class="support-title">あああああああああ</p>
      <p class="support-des">あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ。</p>
      <img class="support-img" src="~assets/images/00027.png" alt="">
    </div>
    <div class="support-sec-01">
      <p class="support-title">ああああ</p>
      <p class="support-des">あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
        <img class="support-img" src="~assets/images/00027.png" alt="">
    </div>
    <div class="support-sec-01 sec-02">
      <p class="support-title">ああああ</p>
      <p class="support-des">ああああああああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
        <img class="support-img" src="~assets/images/00027.png" alt="">
    </div>
    <div class="support-sec-01">
      <p class="support-title">あああああああああ</p>
      <p class="support-des">あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
        <img class="support-img" src="~assets/images/00027.png" alt="">
    </div>
    </div>
    </div>
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



#container3{
  width: 100vw;
  // background-color: #FFEFEF;
  margin: 0 calc(50% - 50vw);
  box-sizing: border-box;
}
h3{
  font-size: 23px;
  font-weight: bold;
  margin:88px 0 95px 0;
  line-height: 2;
}
.support-sec{
    width: 880px;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    position: relative;

  .sec-02{
    margin-right: 40px;
  }
  > .support-sec-01{
    width: 419px;
  height: 505px;
    background: #fff;
  border-radius: 30px;
  margin-bottom: 185px;
  @include sp{
  width: 351px;
height: auto;
background: #fff;
border-radius: 30px;
margin-bottom: 63px;
  }
  > .support-title{
    color: #EF6687;
    font-size: 24px;
    font-weight: bold;
    position:relative;
    transform: translateY(-50%);
  }
  > .support-des{
      line-height: 2;
    font-size: 16px;
    padding: 0 41px 0 41px;
    text-align: left;
    height: 233px;
    @include sp{
    height: auto;
    padding: 0px;
    width: 294px;
    margin: 0 auto;
    margin-bottom: 15px;
    }
  }
  .support-img{
    width: 419px;
  height: 272px;
  @include sp{
width: 351px;
object-fit: contain;
margin-bottom: -22px;
  }
  }
  }
}
.bg{
    background-color: #FFEFEF;
    width: 100%;
    height: 983px;
    position: absolute;
    top: 1230px;
    left: 0;
}

// ----------------------------
#avater-title{
  @include sp{
    margin-top: -60px;
  }
}

h3{
  @include sp{
   font-size: 16px;
    width: 325px;
    margin: 45px auto 72px;
  }
}

.support-sec{
  @include sp{
  display: block;
  }
}



</style>


