<template>
  <div class="projecte">
    <projecteBasic>
      <template #name>
        <span>联通沃阅读</span>
      </template>
      <template #desc>
        项目从14年开始开发，一直在不断迭代更新，目前有小说阅读模块，听书模块。对接过穿山甲，看广告功能，大数据上报打点功能等，小说阅读模块采用jsp后台模板渲染的技术，听书模块是基于vue从0到1构建，功能包括小说推荐，播放定时，音质选择，集数选择， 最近读播放等。
      </template>
      <template #link>
        联通手厅营业厅-小说。
      </template>
      <!-- <template #difficulty>广告SDK调用，版本兼容，iOS和安卓的兼容</template> -->
      <template #otherName1>项目难点：</template>
      <template #otherContent1>
        <p>1.穿山甲广告SDK调用，和穿山甲广告开发人员的联调。广告的测试，需要上灰度。</p>
        <p>2.手厅版本兼容。8.0和8.0以下的区别很大。</p>
        <p>3.iOS和安卓的兼容，手厅的api在iOS上和安卓上有着一些明显的调用差异。</p>
        <p>4.和联通手厅开发人员的沟通以及功能的联调。</p>
      </template>
      <template #dec>jsp， jQuery</template>
    </projecteBasic>

    <projecteBasic>
      <template #name>个人博客系统</template>
      <template #link>
        <a href="http://www.97blognb.cn/#/" class="projecte-link">http://www.97blognb.cn/#/</a>
      </template>
      <template #desc>使用nginx搭建服务，用于记录个人技术，心得 ， 生活， 博客文章的个人网站， 网站主体色采用白色， 清爽简洁。网站的导航以及侧边栏展示实现了可配置化和可自由组合化，也就是说，可以在后台管理系统中任意添加多个导航，可以在后台管理系统中任意见面配置侧边栏的展示部分，项目有三端， 门户端， 后台管理端(<a class="projecte-link" href="http://www.97blognb.cn/blog-admin/#/login">http://www.97blognb.cn/blog-admin/#/login</a>)以及服务端，门户端负责展示， 管理端负责文章的增删改查以及博客的运营。使用node + exress + mysql 构建服务端</template>
      <template #difficulty>管理管的登录token验证，时效验证， 服务端项目搭建，分页方法封装，mysql存储，sql语句的封装</template>
      <template #dec>vue，axios, vue-cli，vue-router，vuex，scss，element-ui，core-js，node，express，mysql，nginx</template>
      <template #github>
        <a href="https://github.com/luyibiao/blog-website-node" class="projecte-link">https://github.com/luyibiao/blog-website-node</a>
      </template>
    </projecteBasic>

    <projecteBasic>
      <template #name>ui组件库（vi-element-vue）</template>
      <template #link>
        <a href="https://luyibiao.github.io/vi/dist/#/" class="projecte-link">https://luyibiao.github.io/vi/dist/#/</a>
      </template>
      <template #desc>个人开源项目，基于vue开发的后台管理系统ui库，项目采用vue-cli，markdown-it，markdown-it-container搭建脚手架，markdown-it用于解析markdown文件，markdown-it-container用于创建markdown容器。项目内部使用scss作为css预编译处理器，基于vue来编写组件源码。库的主题采用友好柔和的蓝色，可通过自己引入的scss文件来覆盖库原本的主题，可手动配置zIndex层级以及其他的一些初始配置，库的核心文件夹有四个，一个demo展示，一个markdown配置，一个静态资源存放处，一个组件源码放置处。组件库的核心功能主要为表单组件，在校验，错误收集这一块，做到了完全的可配置化，既能在外部以自定义的方式弹出又能在内部以组件定好的规则展示出，只需要向每一个表单项传入校验的正则， 就能校验表单项的内容， 而不需要在外面自定义逻辑，在一定程度上减小了开发生产力。</template>
      <template #dec>vue， vue-router, webpack. webpack-cli, scss, markdown，vue-cli。</template>
      <template #github>
        <a href="https://github.com/luyibiao/vi" class="projecte-link">https://github.com/luyibiao/vi</a>
      </template>
    </projecteBasic>

    <projecteBasic>
      <template #name>popper插件（v-poppers）</template>
      <template #link>
        <a href="https://www.npmjs.com/package/v-poppers" class="projecte-link">https://www.npmjs.com/package/v-poppers</a>
      </template>
      <template #desc>一个popper容器浮动库，基于构建工具开发的一个容器浮动插件，给定一个元素（比如一个按钮）和一个描述它的工具提示元素，Popper会自动将弹框提示放在元素附近的正确位置。它将定位从文档流中“弹出”并浮动在目标元素附近的任何UI元素。它可以确保与被跟踪元素在一起，比如下拉菜单，弹出时的编辑检测。</template>
      <template #dec>webpack，es6。</template>
      <template #github>
        <a href="https://github.com/luyibiao/popper" class="projecte-link">https://github.com/luyibiao/popper</a>
      </template>
    </projecteBasic>

    <projecteBasic>
      <template #name>中华联合湖南财险公众号星级专享</template>
      <template #link>
        <a href="https://m.chehaha.net/cicp/" class="projecte-link">https://m.chehaha.net/cicp/</a>（微信链接， 需在微信里打开）
      </template>
      <template #desc>目前承接的是中华联合湖南分公司下的车险服务，是汽车4S店电商B2C服务平台，致力于匹配4S店和车主信息资源，为4S店提供更便捷的客源导流预约服务，主营业务包括：汽车维修保养线上预约服务，机动车辆年检年审线上预约服务，其所有业务包括道路救援，车务年检代办，安全检测，代驾，违章查询， 洗车维修保养，油漆面查找附近商家等可进行配置的微信h5线上平台。项目基于webpack4搭建脚手架，将vue和vant的源码和一些常用设置上传到公司cdn服务器上，在通过cdn的方式引入到项目中去。</template>
      <template #dec>vue，vuex， axios，vue-router，vant，wxsdk，scss，webpack。</template>
      <template #otherName>负责内容：</template>
      <template #otherContent>
        <p>1.项目脚手架的构成</p>
        <p>2.解决不同手机微信浏览器的兼容性问题</p>
        <p>3.抽离项目可维护的常用组件</p>
        <p>4.解决项目中的一些难点和痛点</p>
      </template>
      <template #otherName1>项目难点：</template>
      <template #otherContent1>
         <div>
          <div>
            <p>1.A页面提交表单，需要到B页面获取数据，并将数据返回给A页面，如果从B页面返回给A页面，那么A页面此前所填的数据都将会被重置，而项目不使用keep-Alive来缓存路由。</p>
            <p>解决方式：以弹框 + hash的方式来模拟路由，当用户点击跳转B页面时，实际弹出的是一个全屏的弹框（可配置），将B页面的内容以组件的方式动态传入给这个弹框，当弹框关闭时，将返回一个promise对象，所拿到的数据在then方法里以参数的形式呈现处理来。而hash存在的作用是为了防止用户物理返回。</p>
          </div>
          <p>2.vant的时间选择器划动不流畅，基于vant的时间选择器bug和用户体验效果，自己便封装了时间选择器组件，功能跟vant相同，体验效果更佳。</p>
          <p>3.仓储的刷新，需要做安卓和ios的兼容。</p>
          <p>4.每个车主最多可添加三辆车，切换到不同车牌下，对仓储数据的刷新和优惠券的获取。</p>
          <p>5.需应用到多个客户端，后台管理系统根据渠道码可对业务进行配置，在首页需动态的显示相应业务。</p>
        </div>
      </template>
    </projecteBasic>

    <projecteBasic>
      <template #name>星城园丁志愿者项目</template>
      <template #desc>星城园丁由长沙市公安局与互联网公司合作打造的互联网 + 群防群治平台，公司与长沙市公安局合作，着力打造政府政策激励与市场的物质奖励的“双轮驱动模式”，开发模块名为交通事故远程处理志愿者的项目，协助交警解决一些交通事故，让事故车主走线上平台，以尽快的方式来承担此次事故中的责任，此项目中我担任前端开发并架构，此项目是内嵌项目，嵌套到为星城园丁App里的H5项目， 目前为长沙星城园丁志愿者所使用。</template>
      <template #dec>vue，vuex axios，vue-router，vant，scss。</template>
      <template #difficulty>上传图片需调用星城园丁SDK。</template>
    </projecteBasic>

    <projecteBasic>
      <template #name>中国人寿财险湖南省分公司公众号</template>
      <template #desc>为中国人寿湖南省分公司开发的一个公众号， 其业务包括道路救援， 家政服务， 车务代办， 出险代步，代驾，洗车， 维修，预约保养，安全检测， 违章查询等功能。</template>
      <template #dec>vue, vux, vuex, axios, vue-router。</template>
      <template #otherName>负责内容：</template>
      <template #otherContent>
        <p>1.维护已有代码</p>
        <p>2.开发新需求</p>
        <p>3.修复bug</p>
      </template>
    </projecteBasic>

    <projecteBasic>
      <template #name>O2O模式小程序项目（通洗生活）</template>
      <template #desc>为平台化的项目，采用B2B的商业模式，不同的商家可以入驻我们的平台，入驻的商家都有一个为其定制的后台管理系统，商家在后台管理系统根据不同的模板可以生成小程序不同厂商之间的个性化页面，小程序项目是针对所用通洗软件的商家下的客户而开发的，客户可在小程序上预约下单，将衣服或要洗涤的衣物放到附近的智能柜，或者由顺丰快递员上门取件，送去洗衣商家的一个线上平台。项目包含有商城，物流系统，友商系统。</template>
      <template #dec>vue, vux, vuex, axios, vue-router。</template>
      <template #otherName>负责内容：</template>
      <template #otherContent>
        <p>1.主导小程序前端开发，使用原生开发项目业务， 调用后台API，实现ui设计好的功能。</p>
        <p>2.封装功能视图组件。</p>
        <p>3.指导后端协助开发小程序。</p>
      </template>

      <template #otherName1>项目难点：</template>
      <template #otherContent1>
        <p>1.用的原生开发小程序，一些组件需要自己封装。</p>
        <p>2.微信支付，卡券活动， 分享海报并截屏，派送员实时定位。</p>
        <p>3.全局样式替换，根据不同的模板生成不同的厂商个性化页面。</p>
      </template>
    </projecteBasic>
  </div>
</template>

<script>
import individualWrap from './individual/individual-wrap'
import individualItem from './individual/individual-item'

import projecteBasic from './projecte-basic'
export default {
  components: {
    individualWrap,
    individualItem,
    projecteBasic
  },
  data() {
    return {
      
    }
  },
}
</script>

<style lang="scss">
  .projecte {
    .projecte-name-work {
      font-weight: 400;
      color: #999d9c;
      font-size: 13px;
      margin-left: 20px;
      vertical-align: top;
    }
  }
</style>