<template>
  <div>

    <header class="masthead">
                <div class="site-heading pc-only">
                  <p>ああああああああああ・ああああの<br>
                      新しい働き方を</p>       
              </div>
                <div class="site-heading sp-only">
                  <p>ああああああああああ<br>ああああの<br>
                      新しい働き方を</p>       
              </div>
    </header>

</div>
</template>


<style lang="scss" scoped>

$sp:375px;
 
@mixin sp {
  @media screen and (max-width: ($sp)) {
    @content;
  }
}

$main-color:#ef6687;

// #mainNav {
//     position: absolute;
//     border-bottom: 1px solid #e9ecef;
//     background-color: white;
//     font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
//   }

  header.masthead {
    margin-bottom: 50px;
    background-image: url(~assets/images/00021.png);
    background-size: contain;
    background-position: center bottom;
    position: relative;
    height: 550px;
    background-repeat: no-repeat;
    width: 100%;
    @include sp{
    background-image: url(~assets/images/00029.png);
    background-size: contain;
    background-position: center;
    width: 375px;
    height: 243px;
    padding: 250px 0;
    }
  }

 .site-heading{
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    z-index: 1;
    display: flex;
    justify-content: center;
    color: #fff;
    text-align: center;
    padding: 250px;
    @include sp{
      padding: 190px 70px;
    }
  }

  .site-heading::before{
    width: 100%;
    height: 550px;
    z-index: 0;
    content: "";
    display: block;
    position: absolute;
    top: 0;
    left: 0;
    background-color:#212529;
    opacity: 0.2;
    @include sp{
      height: 370px;
    }
  }

  .site-heading p{
    font-size: 50px;
    font-weight: bold;
    line-height: 1.5;
    z-index: 1;
    position: relative;
    @include sp{
      font-size: 25px;
      width: 250px;
      margin: 0 auto;
    }
  }

  .pc-only{
    @include sp{
      display: none;
    }
  }


.sp-only{
  display: none;
  @include sp{
    display: inline;
  }
}

  </style>