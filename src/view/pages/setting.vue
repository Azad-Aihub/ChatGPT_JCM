<template>
  <div class="setting">
    <el-container>
      <el-header>
        <transition name="el-zoom-in-top">
          <div v-show="show" class="transition-box">
            <h3>使用小提示</h3>
          </div>
        </transition>
      </el-header>
      <el-main>
        <transition name="el-zoom-in-top">
          <div v-show="show" class="transition-box">
            <span>
              本站仅供<a href="https://t.zsxq.com/0cy1WzxXu" target="_blank">【不止GPT】星球成员</a>内部使用。<br>现已接入OpenAI的Models API、Completions API、Chat API、Audio API、Images API、Files API、Fine-tunes API等。<br>右侧填入API KEY后，“模型”处自动检索当前可用模型。<br>需要保存当前会话内容，请点击“创建会话”--“导出会话”。
            </span>
            <div>
              <a href="http://www.azad.asia/" target="_blank">我的主页</a>---<a href="https://faka.azad.asia/" target="_blank">我的小店</a>
            </div>
          </div>
        </transition>
      </el-main>
    </el-container>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      show: false,
    };
  },
  mounted() {
    this.show = true;
  },
};
</script>

<style>
  .transition-box {
    text-align: center;
    margin-top: 5%;
    color: #F2F6FC;
    font-size: 30px;
  }
  h1 {
    color: aliceblue;
    font-size: 80px;
  }
  a {
    text-decoration: none;
    color: #67C23A;
  }
</style>
