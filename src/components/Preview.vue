<template>
  <el-row class="pre">
    <el-col :span="8" v-for="site in sites" :key="site.name" :offset="1" class="card">
      <el-card :body-style="{ padding: '0px' }" shadow="hover">
        <div style="padding: 14px;">
          <span>{{site.name}}</span>
          <div class="bottom clearfix">
            <time class="time">{{ currentDate }}</time>
            <el-button type="text" class="button">操作按钮</el-button>
          </div>
        </div>
        <el-divider></el-divider>
        <div class="pre-text">
            <p >预览的文字.好了，node环境已经安装成功，由于有些npm有些资源被屏蔽或者是国外资源的原因，经常会导致用npm安装依赖包的时候失败,所以还需要安装npm的国内镜像----cnpm.....</p>
        </div>
        <div class="img">
          <img src="https://shadow.elemecdn.com/app/element/hamburger.9cf7b091-55e9-11e9-a976-7f4d0b07eef6.png" class="image">
        </div>
      </el-card>
    </el-col>
  </el-row>

</template>

<script>
    export default {
        name: "Preview",
        data (){
          return{
            currentDate: new Date(),
            sites: [
              { name: 'Runoob' },
              { name: 'Google' },
              { name: 'Taobao' }
            ]
          }
        }
    }
</script>

<style scoped>
  .time {
    font-size: 13px;
    color: #999;
  }

  .bottom {
    margin-top: 13px;
    line-height: 12px;
  }

  .button {
    padding: 0;
    float: right;
  }

  .image {
    float:right;
    display:block;
  }

  .clearfix:before,
  .clearfix:after {
    display: table;
    content: "";
  }

  .clearfix:after {
    clear: both
  }
  .pre{
    margin-top:40px;
    width: 50%;
  }
  .card{
    width: 100%;
    height: 400px;
    clear:both;
    margin-top:15px;
  }
  .pre-text{
    float:left;
    width: 50%;
    margin:0;
    border:0;
    padding:0;
  }
  .img{
    float:right;
    width:50%;
    margin:0;
    border:0;
    padding:0;
  }
</style>
