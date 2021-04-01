<template>
  <div class="home-main">
    <div class="header">
      <span class="hedaer-name">陆益标</span>
      <span class="header-direction">求职意向：前端开发</span>
      <div class="header-img">
      </div>
    </div>

    <!--基本信息-->
    <div class="home-basic-info">
      <div class="basic_item" v-for="(item, index) in basicList" :key="index">
        <span>{{item.name}}：</span>
        <span>{{item.val}}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      basicList: [{
        name: '电话',
        val: '18274850343'
      }, {
        name: '邮箱',
        val: '1739717921@qq.com'
      }, {
        name: '状态',
        val: '离职-随时到岗'
      }, {
        name: '性别',
        val: '男'
      }]
    }
  },
}
</script>

<style lang="scss">
  .home-main {
    width: 900px;
    margin: 0 auto 0;
    background-color: #f2f0f5;
    padding: 60px 0;
    color: #333;
    .header {
      position: relative;
      width: 85%;
      margin-left: auto;
      border-top-left-radius: 12px;
      border-bottom-left-radius: 12px;
      background-color: #6dc7cf;
      padding: 20px 0 20px 30px;
      box-sizing: border-box;
      line-height: 1;
      .hedaer-name {
        color: #fff;
        font-size: 30px;
        font-weight: 500;
      }
      .header-direction {
        margin-left: 20px;
        color: #fff;
        font-size: 25px;
      }
      .header-img {
        position: absolute;
        width: 120px;
        height: 120px;
        background-color: red;
        border-radius: 50%;
        right: 30px;
        top: 50%;
        transform: translateY(-50%);
        background-repeat: no-repeat;
        background-size: contain;
        background-image: url('~@/assets/imgs/header-img.jpg');
        box-shadow: #666 0px 0px 12px;
      }
    }

    .home-basic-info {
      width: 85%;
      margin: 40px 0 20px auto;
      display: flex;
      flex-wrap: wrap;
      .basic_item {
        flex: 1;
        flex-basis: 50%;
        font-size: 15px;
        &:nth-child(n + 3) {
          margin-top: 18px;
        }
      }
    }
  }
</style>
