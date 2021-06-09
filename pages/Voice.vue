<template>
    <div class="container row d-flex justify-content-center align-items-center">
    <Title class="text-center">社員の声</Title>

    <div class="voice">

      <div class="voice-sec">
        <div>
          <img class="voice-img" src="~assets/images/00028.png" alt="">
        </div>
        <div class="right">
          <p class="name">あああああああああああああ<span>あああああああああああああ</span></p>
          <div class="voice-des">
          <p>あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
          </div>
        </div>
      </div>
      <div class="voice-sec voice-wrap">
        <div>
          <img class="voice-img " src="~assets/images/00028.png" alt="">
        </div>
        <div class="right">
          <p class="name">あああああああああああああ<span>あああああああああああああ</span></p>
          <div class="voice-des">
          <p>あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
          </div>
        </div>
      </div>
      <div class="voice-sec">
        <div>
          <img class="voice-img" src="~assets/images/00028.png" alt="">
        </div>
        <div class="right">
         <p class="name">あああああああああああああ<span>あああああああああああああ</span></p>
          <div class="voice-des">
          <p>あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
          </div>
        </div>
      </div>
      <div class="voice-sec voice-wrap">
        <div>
          <img class="voice-img" src="~assets/images/00028.png" alt="">
        </div>
        <div class="right">
          <p class="name">あああああああああああああ<span>あああああああああああああ</span></p>
          <div class="voice-des">
          <p>あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
          </div>
        </div>
      </div>
      <div class="voice-sec">
        <div>
          <img class="voice-img" src="~assets/images/00028.png" alt="">
        </div>
        <div class="right">
         <p class="name">あああああああああああああ<span>あああああああああああああ</span></p>
          <div class="voice-des">
          <p>あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
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

.row{
  min-height: 100vh;
}

.voice{
  margin-top: 80px;
}

.voice-sec{
  background-color: #f2f2f2;
  display: flex;
  width: 1000px;
  padding:60px 30px;


  .voice-img{
    width: 256px;
  }

  .right{
    margin-left: 30px;
  }
  .name{
    color: #ef6687;
    font-weight: bold;
    font-size: 23px;
    border-bottom: 1px solid #ef6687;
    @include sp{
      font-size: 22px;
    }
    span{
      font-weight: bold;
      font-size: 18px;
      color: #454545;
      margin-left: 30px;
      @include sp{
        display: inline-block;
        margin-left: 0px;
      }
    }
  }

  .voice-des{
    font-size: 18px;
    background-color: #fff;
    border-radius: 20px;
    padding: 20px 20px 5px 20px;

    @include sp{
      width: 351px;
    }
   

    .voice-des p{
      line-height: 1.7;
    }

 }
}

.voice-sec:nth-child(even) {
  flex-direction: row-reverse;
}

.right:nth-child(even){
  margin: 30px;
}

.voice-wrap{
  background-color: #FEFFD3;
}

.voice-sec{
  @include sp{
    width: 375px;
    display: block;

  }
}

</style>