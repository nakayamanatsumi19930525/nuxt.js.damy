<template>
  <div class="main-title">
    <slot>タイトル</slot>
  </div>
</template>

<style scoped>
.main-title{
  background-color: red;
  border-radius: 30px 0 30px 0;
  padding: 3px;
  width: 300px;
  color: #fff;
  font-weight: bold;
  font-size: 25px;
  margin: 0 auto;
}
</style>