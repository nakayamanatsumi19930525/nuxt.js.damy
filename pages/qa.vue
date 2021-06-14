<template>
    <div class="container row d-flex justify-content-center align-items-center">
    <Title class="text-center qa-title">Q&A</Title>

  <div class="qa-section">
    <div class="qa">
      <div class="question">
        <p class="qa-main">Q</p>
        <p class="question-p">かっっっっっっっっっっっっっっっっっっっっっっっっっっっっっっっっっっっっk</p>
      </div>
      <div class="answer">
        <p class="qa-main answer-main">A</p>
        <p class="answer-p">うううううううううううううううううううううううううううううううううううううううううう</p>
      </div>
      <div class="answer">
        <p class="qa-main answer-main">A</p>
        <p class="answer-p">あああああああああああああああああああああああああああああああああああああああああ</p>
      </div>
    </div>
    <div class="qa">
      <div class="question">
        <p class="qa-main">Q</p>
        <p class="question-p">あああああああああああああああああああああああああああああああああああああああああ</p>
      </div>
      <div class="answer">
        <p class="qa-main answer-main">A</p>
        <p class="answer-p">あああああああああああああああああああああああああああああああああああああああああ</p>
      </div>
    </div>
    <div class="qa">
      <div class="question">
        <p class="qa-main">Q</p>
        <p class="question-p">あああああああああああああああああああああああああああああああああああああああああ</p>
      </div>
      <div class="answer">
        <p class="qa-main answer-main">A</p>
        <p class="answer-p">あああああああああああああああああああああああああああああああああああああああああ</p>
      </div>
    </div>
    <div class="qa">
      <div class="question">
        <p class="qa-main">Q</p>
        <p class="question-p">あああああああああああああああああああああああああああああああああああああああああ</p>
      </div>
      <div class="answer">
        <p class="qa-main answer-main">A</p>
        <p class="answer-p">あああああああああああああああああああああああああああああああああああああああああ</p>
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

.qa-section{
  margin-bottom: 180px;
  @include sp{
    width: 375px;
    margin-bottom: 0px;
    padding: 0 20px;
  }
}

.qa{
  margin-bottom: 40px;
  margin-top: 75px;
  position: relative;
  // position: absolute;
}

.qa::before{
  content: "";
  position: absolute;
  width: 1000px;
  height: 1px;
  background-color: #c7c7c7;
    top: -45px;

  @include sp{
    width: 351px;
  }
}

.qa:last-child::after {
  content: "";
  position: absolute;
  width: 1000px;
  height: 1px;
  background-color: #c7c7c7;
  bottom: -100px;
  @include sp{
    display: none;
  }
}

.question{
  display: flex;
  align-items: center;
  width: 1000px;
  margin-bottom: 20px;
  margin-top: 30px;

    @include sp{
      align-items: end;
    }
  

  .question-p{
    font-size: 23px;
    font-weight: bold;
    margin-left: 50px;

    @include sp{
    width: 302px;
    font-size: 16px;
    margin-left:7px;
    }
  }
}


.qa-main{
    font-weight: bold;
    font-size: 40px;
    background-color: red;
    width: 72px;
    height: 72px;
    line-height: 72px;
    text-align: center;
    color: #fff;

    @include sp{
    width: 41px;
    height: 41px;
    font-size: 23px;
    line-height: 41px;
    }
}

.answer{
  display: flex;
  align-items: center;

  .answer-main{
    color: #ef6687;
    background-color: #fff;
    border: 1px solid;
}

  .answer-p{
    margin-left: 50px;

    @include sp{
    width: 302px;
    margin-left: 7px;
    }
  }

}

.qa-title{
  margin-bottom: 77px;
}


</style>