<template>
  <el-row class="home" :gutter="20">
    <!-- 左侧列，包含用户信息卡片和表格 -->
    <el-col :span="8" style="margin-top: 20px">
      <div class="card">
        <div class="bg"></div> <!-- 卡片背景 -->
        <div class="blob"></div> <!-- 动画球体 -->
        <el-card>
          <div class="user">
            <img :src="getImageUrl('logo_o')" class="logo_o" /> <!-- 用户Logo -->
            <div class="user-info">
              <p style="color:#ffe0c8">天资聪颖</p>
              <p style="color:#FF3D3D">是天资聪颖呀</p> <!-- 用户角色 -->
            </div>
          </div>
        </el-card>
      </div>

      <!-- 用户数据表格 -->
      <el-card class="user-table" style="height: 400px; top:-40px">
  
        <div class="card" style="height: 400px; background-color: #354656;  font-weight: bold;  ">
          <section class="landscape-section ">
            <div class="sky"></div>
            <div class="sun"></div>
            <div class="hill-1"></div>
            <div class="hill-2"></div>
            <div class="ocean">
              <div class="reflection"></div>
              <div class="reflection"></div>
              <div class="reflection"></div>
              <div class="reflection"></div>
              <div class="reflection"></div>
              <div class="shadow-hill-1"></div>
              <div class="shadow-hill-2"></div>
            </div>
            <div class="hill-3"></div>
            <div class="hill-4"></div>
            <div class="tree-1">
              <svg
                stroke-width="0.00064"
                stroke="#b77873"
                fill="#b77873"
                xml:space="preserve"
                viewBox="0 0 64.00 64.00"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                xmlns="http://www.w3.org/2000/svg"
                id="Layer_1"
                version="1.0"
              >
                <g stroke-width="0" id="SVGRepo_bgCarrier"></g>
                <g
                  stroke-linejoin="round"
                  stroke-linecap="round"
                  id="SVGRepo_tracerCarrier"
                ></g>
                <g id="SVGRepo_iconCarrier">
                  <path
                    d="M32,0C18.148,0,12,23.188,12,32c0,9.656,6.883,17.734,16,19.594V60c0,2.211,1.789,4,4,4s4-1.789,4-4v-8.406 C45.117,49.734,52,41.656,52,32C52,22.891,46.051,0,32,0z"
                    fill="#b77873"
                  ></path>
                </g>
              </svg>
            </div>
            <div class="tree-2">
              <svg
                stroke-width="0.00064"
                stroke="#b77873"
                fill="#b77873"
                xml:space="preserve"
                viewBox="0 0 64.00 64.00"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                xmlns="http://www.w3.org/2000/svg"
                id="Layer_1"
                version="1.0"
              >
                <g stroke-width="0" id="SVGRepo_bgCarrier"></g>
                <g
                  stroke-linejoin="round"
                  stroke-linecap="round"
                  id="SVGRepo_tracerCarrier"
                ></g>
                <g id="SVGRepo_iconCarrier">
                  <path
                    d="M32,0C18.148,0,12,23.188,12,32c0,9.656,6.883,17.734,16,19.594V60c0,2.211,1.789,4,4,4s4-1.789,4-4v-8.406 C45.117,49.734,52,41.656,52,32C52,22.891,46.051,0,32,0z"
                    fill="#b77873"
                  ></path>
                </g>
              </svg>
            </div>
            <div class="tree-3">
              <svg
                version="1.0"
                id="Layer_1"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                viewBox="0 0 64.00 64.00"
                xml:space="preserve"
                fill="#a16773"
                stroke="#a16773"
                stroke-width="0.00064"
              >
                <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                <g
                  id="SVGRepo_tracerCarrier"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                ></g>
                <g id="SVGRepo_iconCarrier">
                  <path
                    fill="#a16773"
                    d="M32,0C18.148,0,12,23.188,12,32c0,9.656,6.883,17.734,16,19.594V60c0,2.211,1.789,4,4,4s4-1.789,4-4v-8.406 C45.117,49.734,52,41.656,52,32C52,22.891,46.051,0,32,0z"
                  ></path>
                </g>
              </svg>
            </div>
            <div class="filter"></div>
          </section>

          <section class="content-section">
            <div class="weather-info">
              <div class="left-side">
                <div class="icon">
                  <svg
                    stroke="#000000"
                    xmlns="http://www.w3.org/2000/svg"
                    fill="none"
                    viewBox="0 0 24 24"
                  >
                    <g stroke-width="0" id="SVGRepo_bgCarrier"></g>
                    <g
                      stroke-linejoin="round"
                      stroke-linecap="round"
                      id="SVGRepo_tracerCarrier"
                    ></g>
                    <g id="SVGRepo_iconCarrier">
                      <path
                        stroke-linecap="round"
                        stroke-width="1.5"
                        stroke="#ffffff"
                        d="M22 14.3529C22 17.4717 19.4416 20 16.2857 20H11M14.381 9.02721C14.9767 8.81911 15.6178 8.70588 16.2857 8.70588C16.9404 8.70588 17.5693 8.81468 18.1551 9.01498M7.11616 11.6089C6.8475 11.5567 6.56983 11.5294 6.28571 11.5294C3.91878 11.5294 2 13.4256 2 15.7647C2 18.1038 3.91878 20 6.28571 20H7M7.11616 11.6089C6.88706 10.9978 6.7619 10.3369 6.7619 9.64706C6.7619 6.52827 9.32028 4 12.4762 4C15.4159 4 17.8371 6.19371 18.1551 9.01498M7.11616 11.6089C7.68059 11.7184 8.20528 11.9374 8.66667 12.2426M18.1551 9.01498C18.8381 9.24853 19.4623 9.60648 20 10.0614"
                      ></path>
                    </g>
                  </svg>
                </div>
                <p>Cloudy</p>
              </div>
              <div class="right-side">
                <div class="location">
                  <div>
                    <svg
                      version="1.0"
                      id="Layer_1"
                      xmlns="http://www.w3.org/2000/svg"
                      xmlns:xlink="http://www.w3.org/1999/xlink"
                      width="64px"
                      height="64px"
                      viewBox="0 0 64 64"
                      xml:space="preserve"
                      fill="#ffffff"
                      stroke="#ffffff"
                    >
                      <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
                      <g
                        id="SVGRepo_tracerCarrier"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      ></g>
                      <g id="SVGRepo_iconCarrier">
                        <path
                          fill="#ffffff"
                          d="M32,0C18.746,0,8,10.746,8,24c0,5.219,1.711,10.008,4.555,13.93c0.051,0.094,0.059,0.199,0.117,0.289l16,24 C29.414,63.332,30.664,64,32,64s2.586-0.668,3.328-1.781l16-24c0.059-0.09,0.066-0.195,0.117-0.289C54.289,34.008,56,29.219,56,24 C56,10.746,45.254,0,32,0z M32,32c-4.418,0-8-3.582-8-8s3.582-8,8-8s8,3.582,8,8S36.418,32,32,32z"
                        ></path>
                      </g>
                    </svg>
                    <span>Spain</span>
                  </div>
                </div>
                <p>Monday, 4th May</p>
                <p class="temperature">24°C</p>
              </div>
            </div>
            <div class="forecast">
              <div>
                <p style="color:#FF3D3D">Tuesday, 5th May</p>
                <p style="color:#FF3D3D">24°C</p>
              </div>
              <div class="separator"></div>
              <div>
                <p style="color:#FF3D3D">Wednesday, 6th May</p>
                <p style="color:#FF3D3D">26°C</p>
              </div>
              <div class="separator"></div>
              <div>
                <p style="color:#FF3D3D">Thursday, 7th May</p>
                <p style="color:#FF3D3D">22°C</p>
              </div>
            </div>
          </section>
        </div>
      </el-card>
    </el-col>

    <!-- 右侧列，包含欢迎信息和图表 -->
    <el-col :span="16" style="margin-top:20px">
      <el-card class="body-style e-card" style="background-color: #1d2e3d">
        <!-- 添加在这里 -->
        <div class="ccard">
        <p class="time-text"><span>11:11</span><span class="time-sub-text">PM</span></p>
<p class="day-text">Wednesday, June 15th</p>
<svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 16 16" stroke-width="0" fill="currentColor" stroke="currentColor" class="moon"><path d="M6 .278a.768.768 0 0 1 .08.858 7.208 7.208 0 0 0-.878 3.46c0 4.021 3.278 7.277 7.318 7.277.527 0 1.04-.055 1.533-.16a.787.787 0 0 1 .81.316.733.733 0 0 1-.031.893A8.349 8.349 0 0 1 8.344 16C3.734 16 0 12.286 0 7.71 0 4.266 2.114 1.312 5.124.06A.752.752 0 0 1 6 .278z"></path><path d="M10.794 3.148a.217.217 0 0 1 .412 0l.387 1.162c.173.518.579.924 1.097 1.097l1.162.387a.217.217 0 0 1 0 .412l-1.162.387a1.734 1.734 0 0 0-1.097 1.097l-.387 1.162a.217.217 0 0 1-.412 0l-.387-1.162A1.734 1.734 0 0 0 9.31 6.593l-1.162-.387a.217.217 0 0 1 0-.412l1.162-.387a1.734 1.734 0 0 0 1.097-1.097l.387-1.162zM13.863.099a.145.145 0 0 1 .274 0l.258.774c.115.346.386.617.732.732l.774.258a.145.145 0 0 1 0 .274l-.774.258a1.156 1.156 0 0 0-.732.732l-.258.774a.145.145 0 0 1-.274 0l-.258-.774a1.156 1.156 0 0 0-.732-.732l-.774-.258a.145.145 0 0 1 0-.274l.774-.258c.346-.115.617-.386.732-.732L13.863.1z"></path></svg>
        </div>
      </el-card>

      <!-- ECharts图表容器 -->
      <div :class="className" :style="{ height: height, width: width }" ref="chartRef"></div>
    </el-col>
  </el-row>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount, watch } from "vue";
import * as echarts from 'echarts';

// 获取图片URL的方法
const getImageUrl = (logo_o) => {
  console.log("Generating image URL for:", logo_o);
  const url = new URL(`../../img/${logo_o}.png`, import.meta.url).href;
  console.log("Generated URL:", url);
  return url;
};

// 图表相关配置
const className = ref('chart'); // 图表类名
const width = ref('100%'); // 图表宽度
const height = ref('480px'); // 图表高度

// X轴数据
const xAxisData = ref(['1', '2', '3', '4', '5', '6', '7', '8', '9', '10']);
// 系列数据
const seriesData = ref([{
  name: 'JAVA',
  type: 'line',
  stack: '总量',
  emphasis: {
    focus: 'series'
  },
  areaStyle: {
     color: '#4a9d9c' // 区域填充颜色
  },
    itemStyle: {
    color: '#61bc84' // 线条颜色
  },
    lineStyle: {
    width: 3 // 线条宽度
  },
  symbol: 'circle', // 数据点形状
  symbolSize: 8, // 数据点大小
  data: [67, 3213, 66, 67, 3228, 32, 1410, 2552, 3512, 555]
}, {
  name: 'Vue3',
  type: 'line',
  stack: '总量',
  areaStyle: {
    color:'#FF3D3D'
  },
  emphasis: {
    focus: 'series'
  },
      lineStyle: {
    width: 3 // 线条宽度
  },
      itemStyle: {
    color: '#FF3D3D' 
  },
    symbol: 'circle', // 数据点形状
  symbolSize: 8, // 数据点大小
  data: [120, 2232, 101, 800, 20, 230, 210, 5466, 67, 36]
}]);

// 图表引用
const chartRef = ref(null); // 图表DOM元素引用
let chartInstance = null; // 图表实例

// 监听X轴数据变化并更新图表
watch(xAxisData, (newVal) => {
  if (chartInstance) {
    chartInstance.setOption({
      xAxis: [
        {
          data: newVal
        }
      ]
    });
  }
}, { deep: true });

// 监听系列数据变化并更新图表
watch(seriesData, (newVal) => {
  if (chartInstance) {
    chartInstance.setOption({
      series: newVal
    });
  }
}, { deep: true });

// 初始化图表
const initChart = () => {
  chartInstance = echarts.init(chartRef.value); // 初始化图表实例
  drawChart(); // 绘制图表
};

// 销毁图表实例
const disposeChart = () => {
  if (chartInstance) {
    chartInstance.dispose(); // 销毁图表实例
    chartInstance = null;
  }
};

// 绘制图表
const drawChart = () => {
  chartInstance.setOption({
    tooltip: {
      trigger: 'axis',
      axisPointer: {
        type: 'cross',
        label: {
          backgroundColor: '#6a7985'
        }
      }
    },
    legend: {
      left: 'center'
    },
    toolbox: {
      feature: {
        saveAsImage: {}
      }
    },
    grid: {
      left: '3%',
      right: '4%',
      bottom: '3%',
      containLabel: true
    },
    xAxis: [
      {
        type: 'category',
        boundaryGap: false,
        data: xAxisData.value
      }
    ],
    yAxis: [
      {
        type: 'value'
      }
    ],
    series: seriesData.value
  });
};

// 组件挂载时初始化图表
onMounted(() => {
  initChart();
});

// 组件卸载前销毁图表实例
onBeforeUnmount(() => {
  disposeChart();
});
</script>

<style lang="less" scoped>
.home {
  background-color: #0D1F2D;
  border-radius: 14px;
  height: 90vh;
  .el-col {
    margin-top: 20px;
  }

  .card {
    position: relative;
    width: 400px;
    height: 220px;
    border-radius: 14px;
    z-index: 1111;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

  .bg {
    position: absolute;
    top: 30px;
    left: 8px;
    width: 364px;
    height: 203px;
    z-index: 2;
    background: #354656; /* 背景半透明 */
    backdrop-filter: blur(24px); /* 背景模糊 */
    border-radius: 10px;
    overflow: hidden;
    outline: 2px solid #354656; /* 白色边框 */
    
  }

  .blob {
    position: absolute;
    z-index: 1;
    top: 50%;
    left: 50%;
    width: 139px; 
    height: 110px;
    border-radius: 10%;
    background-color: rgb(0, 255, 247) ;; /* 蓝色圆点 */
    opacity: 1;
    filter: blur(12px); /* 模糊效果 */
    animation: blob-bounce 2s infinite ease; /* 弹跳动画 */
  }

  @keyframes blob-bounce {
    0% {
      transform: translate(-100%, -100%) translate3d(-10%, 0, 0);
    }

    25% {
      transform: translate(-100%, -100%) translate3d(120%, 0, 0);
    }

    50% {
      transform: translate(-100%, -100%) translate3d(120%, 100%, 0);
    }

    75% {
      transform: translate(-100%, -100%) translate3d(-20%, 100%, 0);
    }

    100% {
      transform: translate(-100%, -100%) translate3d(-10%, 0, 0);
    }
  }

  .el-card {
    position: relative;
    z-index: 3;
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px;
    box-sizing: border-box;
    background: transparent;
    border:solid  0px #ffffff ;

    .user {
      display: flex;
      align-items: center;

      .logo_o {
        width: 130px;
        height: 130px;
        border-radius: 50%;
        margin-right: 30px;
      }

      .user-info {
        p {
            font-weight: bold;
          margin-top: 10px;
          font-size: 20px;
        }
      }
    }
  }

  .user-table {
    margin-top: 50px;
    width: 380px;
    height: 400px;
    border-radius: 14px;
    // box-shadow: 20px 20px 60px #bebebe, -20px -20px 60px #ffffff; /* 表格阴影 */
  }

  .body-style{
    display: flex;
    padding: 0;
    height: 220px;
    position: relative;

    width: 100%;
    background: transparent;
    box-shadow: 0px 8px 28px -9px rgba(0,0,0,0.45); /* 卡片阴影 */
    border-radius: 16px;
    overflow: hidden;
  }

  .wave {
    position: absolute;
    width: 640px;
    height: 700px;
    opacity: 0.6;
    left: 0;
    top: 0;
    margin-left: -55%;
    margin-top: -70%;
    background: linear-gradient(744deg,#af40ff,#5b42f3 60%,#00ddeb); /* 渐变背景色 */
  }

  .icon {
    // font-weight: bold;
    width: 2em;
    margin-top: -1em;
    padding-bottom: 1em;
  }

  .infotop {
    text-align: center;
    font-size: 50px;
    position: absolute;
    top: 1.4em;
    left: 0;
    right: 0;
    color: rgb(255, 255, 255);
    font-weight: 600;
  }

  .name {
    font-size: 20px;
    font-weight: bold;
    position: relative;
    top: -10em;
    left: 12em;
    color: #00ddeb;
    text-transform: lowercase;
  }

  .wave:nth-child(2),
  .wave:nth-child(3) {
    position: relative;
    top: 310px;
    left: 350px;
  }

  .playing .wave {
    border-radius: 40%;
    animation: wave 3000ms infinite linear; /* 波浪动画 */
  }

  .wave {
    border-radius: 40%;
    animation: wave 55s infinite linear; /* 波浪动画 */
  }

  .playing .wave:nth-child(2) {
    animation-duration: 3000ms;
  }

  .wave:nth-child(2) {
    animation-duration: 50s;
  }

  .playing .wave:nth-child(3) {
    animation-duration: 5000ms;
  }

  .wave:nth-child(3) {
    animation-duration: 45s;
  }

  @keyframes wave {
    0% {
      transform: rotate(0deg);
    }

    100% {
      transform: rotate(360deg);
    }
  }

  /* From Uiverse.io by KSAplay */
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
  width: 380px;
  height: 260px;
  border-radius: 14px;
  overflow: hidden;
  
  // box-shadow: 12px 12px 0px rgba(0, 0, 0, 0.1);
  background-color: #0D1F2D;

}

/* Landscape section */
.landscape-section {
  position: relative;
  width: 100%;
  height: 100%;
  overflow: hidden;
  // color: #5b42f3;
}

.landscape-section * {
  position: absolute;
}

.sky {
  width: 100%;
  height: 100%;
  background: rgb(247, 225, 87);
  background: linear-gradient(
    0deg,
    rgba(247, 225, 87, 1) 0%,
    rgba(233, 101, 148, 1) 100%
  );
}

.sun {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 45px;
  height: 45px;
  border-radius: 50%;
  background-color: white;
  bottom: 40%;
  left: 23%;
  filter: drop-shadow(0px 0px 10px white);
}

.sun::after {
  position: absolute;
  content: "";
  width: 118%;
  height: 118%;
  border-radius: 50%;
  background-color: white;
  opacity: 0.5;
}

.sun::before {
  position: absolute;
  content: "";
  width: 134%;
  height: 134%;
  border-radius: 50%;
  background-color: white;
  opacity: 0.1;
}

.ocean {
  overflow: hidden;
  bottom: 0;
  width: 100%;
  height: 28%;
  background: rgb(241, 192, 125);
  background: linear-gradient(
    0deg,
    rgba(241, 192, 125, 1) 0%,
    rgba(247, 218, 150, 1) 100%
  );
}

.reflection {
  position: absolute;
  background-color: white;
  opacity: 0.5;
  z-index: 1;
}

.reflection:nth-child(1) {
  width: 40px;
  height: 10px;
  clip-path: polygon(0% 0%, 100% 0%, 50% 20%);
  top: 5%;
  left: 32%;
}

.reflection:nth-child(2) {
  width: 80px;
  height: 15px;
  clip-path: polygon(0% 0%, 100% 0%, 60% 20%, 40% 20%);
  top: 15%;
  left: 39%;
}

.reflection:nth-child(3) {
  width: 60px;
  height: 2px;
  clip-path: polygon(0% 50%, 40% 0%, 60% 0%, 100% 50%, 60% 100%, 40% 100%);
  top: 27%;
  right: 15%;
}

.reflection:nth-child(4) {
  width: 70px;
  height: 2px;
  clip-path: polygon(0% 50%, 40% 0%, 60% 0%, 100% 50%, 60% 100%, 40% 100%);
  top: 37%;
  right: 28%;
}

.reflection:nth-child(5) {
  width: 70px;
  height: 3px;
  clip-path: polygon(0% 50%, 40% 0%, 60% 0%, 100% 50%, 60% 100%, 40% 100%);
  top: 46%;
  right: 8%;
}

.hill-1 {
  right: -25%;
  bottom: 20%;
  width: 150px;
  height: 40px;
  border-radius: 50%;
  background-color: #e6b29d;
}

.shadow-hill-1 {
  right: -25%;
  top: -30%;
  width: 150px;
  height: 40px;
  border-radius: 50%;
  background-color: #f1c7a0;
  opacity: 1;
}

.hill-2 {
  right: -36%;
  bottom: 10%;
  width: 150px;
  height: 80px;
  border-radius: 50%;
  background-color: #c29182;
}

.shadow-hill-2 {
  right: -36%;
  top: -65%;
  width: 150px;
  height: 80px;
  border-radius: 50%;
  background-color: #e5bb96;
  opacity: 1;
}

.hill-3 {
  left: -100%;
  bottom: -28%;
  width: 350px;
  height: 150px;
  border-radius: 50%;
  background-color: #b77873;
  z-index: 3;
}

.tree-1 {
  bottom: 20%;
  left: 3%;
  width: 50px;
  height: 70px;
  z-index: 3;
}

.tree-2 {
  bottom: 14%;
  left: 25%;
  width: 50px;
  height: 70px;
  z-index: 3;
}

.hill-4 {
  right: -100%;
  bottom: -40%;
  width: 350px;
  height: 150px;
  border-radius: 50%;
  background-color: #a16773;
  z-index: 3;
}

.tree-3 {
  bottom: 10%;
  right: 1%;
  width: 65px;
  height: 80px;
  z-index: 3;
}

.filter {
  height: 100%;
  width: 100%;
  background: linear-gradient(
    0deg,
    rgba(255, 255, 255, 1) 0%,
    rgba(255, 255, 255, 0) 40%
  );
  z-index: 5;
  opacity: 0.2;
}

/* Content section */
.content-section {
  width: 100%;
  height: 30%;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.weather-info {
  display: flex;
  align-items: center;
  justify-content: space-around;
  position: absolute;
  text-align: center;
  top: 0;
  right: 0%;
  width: 100%;
  padding-top: 15px;
  color: white;
  z-index: 10;
}

.weather-info .left-side:not(.icon) {
  width: 20%;
  font-size: 11pt;
  font-weight: 600;
  align-self: baseline;
}

.icon {
  display: flex;
  align-items: center;
  justify-content: center;
}

.icon svg {
  width: 40px;
}

.weather-info .right-side {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

.weather-info .right-side p:nth-child(2) {
  font-size: 9pt;
  margin: 0;
  padding: 0;
}

.weather-info .location span {
  font-size: 11pt;
  font-weight: 700;
  text-transform: uppercase;
}

.location {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  width: 100%;
  padding: 0;
  margin: 0;
}

.location svg {
  width: 14px;
  height: auto;
}

.temperature {
  font-size: 20pt;
  font-weight: 700;
  line-height: 30px;
}

.forecast {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-evenly;
  height: 100%;
  width: 100%;
  padding: 10px 25px;
}

.forecast > div {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: lightslategray;
  font-size: 9pt;
}

.separator {
  width: 100%;
  height: 2px;
  background-color: rgb(233, 233, 233);
  border-radius: 1px;
}
}
/* From Uiverse.io by akshat-patel28 */ 
.ccard {
  width: 900px;
  height:190px;
  background: rgb(17, 4, 134);
  border-radius: 15px;
  box-shadow: rgb(0,0,0,0.7) 5px 10px 50px ,rgb(0,0,0,0.7) -5px 0px 250px;
  display: flex;
  color: white;
  justify-content: center;
  position: relative;
  flex-direction: column;
  background: linear-gradient(to right, rgb(20, 30, 48), rgb(36, 59, 85));
  cursor: pointer;
  transition: all 0.3s ease-in-out;
  overflow: hidden;
}

.ccard:hover {
  box-shadow: rgb(0,0,0) 5px 10px 50px ,rgb(0, 255, 247) -5px 0px 250px;
}

.time-text {
  font-size: 70px;
  margin-top: 0px;
  margin-left: 15px;
  font-weight: 600;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

.time-sub-text {
  font-size: 20px;
  margin-left: 5px;
}

.day-text {
  font-size: 25px;
  margin-top: 0px;
  margin-left: 15px;
  font-weight: 500;
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
}

.moon {
  font-size: 50px;
  position: absolute;
  right: 30px;
  top: 30px;
  transition: all 0.3s ease-in-out;
}

.ccard:hover > .moon {
  font-size: 23px;
  color:rgb(0, 255, 247) ;

}


</style>






