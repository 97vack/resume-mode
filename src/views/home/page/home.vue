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

    <!--工作经历-->
    <modeWrap title="专业技能">
      <template>
        <individualWrap>
          <individualItem v-for="(item, index) in majorList" :key="index" :text="item.text"/>
        </individualWrap>
      </template>
    </modeWrap>

    <modeWrap title="工作经历">
      <template>
        <div class="work-wrap" v-for="(item, index) in workList" :key="index">
          <div class="work_title">
            <span class="work_title-inner" style="text-align: left;">{{item.title}}</span>
            <span class="work_title-inner">{{item.z}}</span>
            <span class="work_title-inner">{{item.time}}</span>
          </div>
          <div class="work_content">
            <individualWrap>
              <individualItem v-for="(i, c) in item.children" :key="c" :text="i.text"/>
            </individualWrap>
          </div>
        </div>
      </template>
    </modeWrap>

    <!-- <div style="page-break-after: always;"></div> -->
    
    <modeWrap title="项目经验">
      <template>
        <projecte />
      </template>
    </modeWrap>

    <modeWrap title="社交主页">
      <div class="social-contact">
        <span class="social-contact_label">GitHub：</span>
        <span><a class="social-contact_link" href="https://github.com/luyibiao">https://github.com/luyibiao</a></span>
      </div>
      <div class="social-contact">
        <span class="social-contact_label">个人网站：</span>
        <span><a class="social-contact_link" href="http://www.97blognb.cn/#/">http://www.97blognb.cn/</a></span>
      </div>
    </modeWrap>

    <modeWrap title="教育经历">
      <div class="education">
        <span>2015/09 - 2018/06</span>
        <span>湖南信息职业技术学院</span>
        <span>计算机软件开发</span>
        <span>全日制统招大专</span>
      </div>
    </modeWrap>
  </div>
</template>

<script>
import modeWrap from '../components/experienceMode/mode-wrap'
import individualWrap from '../components/individual/individual-wrap'
import individualItem from '../components/individual/individual-item'
import projecte from '../components/projecte'
export default {
  components: {
    modeWrap,
    individualWrap,
    individualItem,
    projecte
  },
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
      }],
      majorList: [{
        text: '主攻技术栈为 Vue全家桶以及原生 JavaScript、ES6等，在相关技术有着丰富的开发经验。'
      }, {
        text: '计算机相关专业。'
      }, {
        text: '清晰的组件化思维，可以独立开发高复用性组件。'
      }, {
        text: '使用node.js + express + mysql搭建过个人博客系统。'
      }, {
        text: '个人开源项目。'
      }],
      workList: [{
        title: '江苏中兴华易科技发展有限公司',
        z: '前端开发',
        time: '2020.08 - 2021.04',
        children: [{
          text: '负责联通沃阅读核心业务项目的迭代开发和维护。'
        }, {
          text: '负责项目新需求的评估和评审。'
        }, {
          text: '负责对项目的老模块的重构，将原有的使用老框架的代码逐步换成统一的Vue写法，可以有效的减少后续对老模块的维护成本。'
        }, {
          text: '提取代码组建化，提升开发和维护效率。'
        }]
      }, {
        title: '湖南车哈哈汽车科技股份有限公司',
        z: '前端开发',
        time: '2019.02 - 2020.07',
        children: [{
          text: '基于vue + Element开发后台管理系统。'
        }, {
          text: '基于vue + vant开发公司C端项目。'
        }, {
          text: '构建公司内部Vue技术的UI组件库。'
        }, {
          text: '制定部门的代码风格规范。'
        }, {
          text: '更新迭代公司项目'
        }]
      }, {
        title: '湖南友靠科技有限公司',
        z: '前端开发',
        time: '2017.12 - 2019.02',
        children: [{
          text: '使用vue框架和element-ui开发后台管理系统'
        }, {
          text: '使用vue框架和vux开发公众号'
        }, {
          text: '主导小程序前端开发'
        }, {
          text: '维护已有项目'
        }, {
          text: '与后端开发人员合作完成产品的界面和功能'
        }]
      }]
    }
  },
}
</script>

<style lang="scss">
  .home-main {
    width: 800px;
    margin: 0 auto 0;
    // background-color: #f2f0f5;
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
      margin: 40px 0 60px auto;
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

    .work-wrap {
      .work_title {
        width: 100%;
        display: flex;
        text-align: center;
        font-weight: bold;
        .work_title-inner {
          flex: 1;
        }
      }
      .work_content {
        margin-top: 20px;
        .individual-item {
          font-size: 14px;
        }
      }
    }
    .work-wrap + .work-wrap {
      margin-top: 30px;
    }

    .social-contact {
      .social-contact_label {
        font-weight: bold;
        font-size: 15px;
      }
      .social-contact_link {
        font-size: 15px;
      }
    }

    .social-contact + .social-contact {
      margin-top: 15px;
    }

    .education {
      display: flex;
      justify-content: space-between;
      font-weight: bold;
    }
  }
</style>
