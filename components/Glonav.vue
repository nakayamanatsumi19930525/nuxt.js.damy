<template>
<div>
 <div id="tabs" class="container">
      <ul class="list">
          <router-link class="nav-link" v-on:click="activetab=1" v-bind:class="[ activetab === 1 ? 'active' : '' ]">TSUTSUMUとは</router-link>
          <router-link class="nav-link" v-on:click="activetab=2" v-bind:class="[ activetab === 2 ? 'active' : '' ]">サポート体制</router-link>
          <router-link class="nav-link" v-on:click="activetab=3" v-bind:class="[ activetab === 3 ? 'active' : '' ]">社員の声</router-link>
          <router-link class="nav-link" v-on:click="activetab=4" v-bind:class="[ activetab === 4 ? 'active' : '' ]">Q&A</router-link>
      </ul>
       <div class="content">
          <div v-show="activetab === 1" class="tabcontent">
              コンテンツ01
          </div>
          <div v-show="activetab === 2" class="tabcontent">
              コンテンツ02
          </div>
          <div v-show="activetab === 3" class="tabcontent">
              コンテンツ03
          </div>
      </div>
  </div>
</div>
</template>



<style lang="scss" scoped>

  .nav-link{
    position: relative;

     &:not(:last-child):before{
    content: "";
    position: absolute;
    bottom: 9px;
    display: inline-block;
    width: 2px;
    height: 25px;
    transform: translate(-50%);
    background-color: #707070;
    right: -20px;
    }
  }

  .list{
    display: flex;
    justify-content: space-between;
    list-style: none;
    margin: 0 auto;
    width: 60%;
    margin-top: -30px;
    font-size: 18px;
    font-weight: bold;
  }

</style>