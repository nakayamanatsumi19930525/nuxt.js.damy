<template>
  <div class="flex items-center min-h-screen bg-black">
    <MainVisual></MainVisual>
    <div class="container-contact mx-auto">
      <div class="max-w-md mx-auto my-10 bg-white p-5 rounded-md shadow-sm">
        <div class="text-center">
           <Title class="text-center contact-title">お問い合わせ</Title>
          <p class="main-des">ああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
        </div>
        <div class="m-7">
          <form>
            <div class="mb-6">
                <th class="block mb-2 text-sm text-gray-600 contact-item contact-left">ご担当者様名（名） <span class="text-xs text-red-500">必須</span></th>
              <input
                id="name"
                type="text"
                name="name"
                placeholder="姓"
                class="w-full px-3 py-2 bg-light placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 contact-right"
              />
            </div>
            <div class="mb-6">
              <th class="block mb-2 text-sm text-gray-600 contact-item contact-left">ご担当者様名（名） <span class="text-xs text-red-500">必須</span></th>
              <input
                id="name"
                type="text"
                name="name"
                placeholder="名"
                class="w-full px-3 py-2 bg-light placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 contact-right"
              />
            </div>
            <div class="mb-6">
              <th class="block mb-2 text-sm text-gray-600 contact-item contact-left">会社もしくはご所属名 <span class="text-xs text-red-500">必須</span></th>
              <input
                id="name"
                type="text"
                name="name"
                placeholder="〇〇〇株式会社"
                class="w-full px-3 py-2 bg-light placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 contact-right"
              />
            </div>
                  <div class="mb-6">
              <th class="block mb-2 text-sm text-gray-600 contact-item contact-left">電話番号 <span class="text-xs text-red-500">必須</span></th>
              <input
                id="phone"
                type="text"
                name="phone"
                placeholder="00-0000-0000"
                class="w-full px-3 py-2 bg-light  placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 contact-right"
              />
            </div>
            <div class="mb-6">
              <th class="block mb-2 text-sm text-gray-600 contact-item contact-left">メールアドレス <span class="text-xs text-red-500">必須</span></th>
              <input
                id="email"
                type="email"
                name="email"
                placeholder="〇〇〇〇〇〇@〇〇〇〇"
                class="w-full px-3 py-2 bg-light placeholder-gray-300 border border-gray-300 rounded-md focus:outline-none focus:ring focus:ring-indigo-100 focus:border-indigo-300 contact-right"
              />
            </div>
      
            <div class="mb-6 textarea">
             <th class="block mb-2 text-sm text-gray-600 contact-item contact-left">備考 <span class="text-xs text-red-500 optional">任意</span></th>
              <textarea
                id="message"
                rows="5"
                name="message"
                placeholder="用途の詳細や、ご意見やご希望などございましたらご自由にご記入ください。"
                class="w-full px-3 py-2 bg-light placeholder-gray-300 border border-gray-300 rounded-md contact-right"
              >
              </textarea>
            </div>

            <div class="mb-6 ">
              <button
                type="submit"
                class="text-center w-full px-3 py-4 font-bold text-white bg-green-500 rounded-md focus:bg-green-600 focus:outline-none contact-btn"
              >
                送信内容を確認
              </button>
            </div>
          </form>
        </div>
        <p class="contact-sub">ああああああああああああああああああああああああああああああああああああああああああああああああああああああ</p>
      </div>
    </div>
  </div>
</template>



<script>
import Title from "~/components/Title.vue";
import MainVisual from "~/components/MainVisual.vue";
export default {
  components: {
    Title,
    MainVisual
  }
};
</script>



<style scoped>

.contact-title{
  margin-top: 82px;
}

.container-contact{
  margin-top: 100px;
}

.main-des{
      font-size: 20px;
    font-weight: bold;
    margin-top: 93px;
    margin-bottom: 116px;
}

.contact-btn{
    background: #3277ad;
    border: none;
    width: 321px;
    height: 78px;
    margin: 0 auto;
    vertical-align: middle;
    border-radius: inherit;
}

input{
   max-width: 584px;
    width: 100%;
    height: 62px;
    margin-bottom: 93px;
  appearance: none;
  -webkit-appearance: none;
    -moz-appearance: none;
}
th{
  font-weight: normal;
  font-size: 18px;
  color: #454545;
  margin-top: 15px;
}

.mb-6{
  display: flex;
  justify-content: center;

}

textarea{
  max-width: 584px;
  width: 100%;
    /* padding: 10px; */
    height: 250px;
    appearance: none;
    -webkit-appearance: none;
    -moz-appearance: none;
}

.contact-left {
    text-align: left;
    width: 30%;
    /* background-color: #eee; */
}

.contact-right {
    width: 70%;
}

.textarea{
  margin-bottom: 138px;
}

.contact-sub{
  text-align: center;
  margin-top: 95px;
}

span{
    width: 63px;
    padding: 4px 0;
    background-color: #ef6687;
    float: right;
    margin-right: 30px;
    border-radius: 30px;
    text-align: center;
    color: #fff;
    font-size: 12px;
}

.optional{
  background-color: #939393;
}
</style>