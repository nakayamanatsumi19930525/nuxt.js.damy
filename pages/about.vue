<template>
<div>
  <MainVisual></MainVisual>
  <div class="tabs">
    <div class="btn-container">
      <button v-for="(tab, index) in tabs"
              :key="tab.id"
              :class="{ active: currentTab === index }"
              @click="currentTab = index">{{ tab.tabName }}</button>
    </div>
    <div class="tab-content">
      <div id="tab-content-0" v-show="currentTab === 0">
       <AvaterGuild></AvaterGuild>
      </div>
      <div v-show="currentTab === 1">
        <Support class="text-center"></Support>
      </div>
      <div v-show="currentTab === 2">
         <Voice></Voice>
      </div>
      <div v-show="currentTab === 3">
        <qa></qa>
      </div>
    </div>
  </div>
</div>
</template>

<script>
import MainVisual from "~/components/MainVisual.vue";
import AvaterGuild from "~/pages/AvaterGuild.vue";
import Support from "~/pages/Support.vue";
import Voice from "~/pages/Voice.vue";
import qa from "~/pages/qa.vue";
export default {
  name: 'tabs',
  data () {
    return {
      currentTab: 0,
      id: 0,
      tabName: "",
      tabs: [
        {id: 1, tabName: 'TSUTSUMUについて'},
        {id: 2, tabName: 'サポート体制'},
        {id: 3, tabName: '社員の声'},
         {id: 4, tabName: 'Q&A'}
      ],
    }
  },
   components: {
    MainVisual,
    AvaterGuild,
    Support,
    Voice,
    qa
  },
}  
</script>

<style lang="scss" scoped>

$sp:375px;
 
@mixin sp {
  @media screen and (max-width: ($sp)) {
    @content;
  }
}


.tabs {
  margin: 10px auto;
  padding: 10px;
  width: 80%;
  height: 80%;
  border-radius: 10px;

  @include sp{
    margin: 0;
    width: 100%;
    margin-top: -120px;
  }
}
h1 p{
  font-family: 'Courier New', Courier, monospace;
}
h1 {
  font-size: 20px;
}
p {
  font-size: 8px;
}
.btn-container {
  display: flex;
  justify-content: center;
}
button {
 width: 18%;
    font-size: 20px;
    text-align: center;
    padding: 3px 10px;
    border: transparent;
    font-size: 16px;
    font-weight: bold;
    color: #707070;
    background-color: unset;
     position: relative;
     outline: none;

    &:not(:last-child):before{
      content: "";
    position: absolute;
    bottom: 1px;
    display: inline-block;
    width: 2px;
    height: 25px;
    transform: translate(-50%);
    background-color: #707070;
    right: 0px;
    }
}
button.active{
  border-bottom: 2px solid lightcoral;
}

.tab-content div {
  padding: 50px;
  background: #ffffff;
  width: 80%;
  margin: 0 auto;
  @include sp{
    padding: 0px;
    width: 100%;
  }
}

#tab-content-0{
  background-color: #FEFFD3;
  margin: 0 calc(50% - 50vw);
  box-sizing: border-box;
  width: 1440px;
  margin-top: 160px;
  margin-bottom: -20px;
}

/* ----------------------------- */

.btn-container{
  @include sp{
    display: none;
  }
}

#tab-content-0{
  @include sp{
    width: 375px;
    margin-top: 0px;
  }
}

#container2{
  @include sp{
    width: 100%;
  }
}


</style>