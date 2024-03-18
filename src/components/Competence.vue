<template>
  <div class="time-capsule">
     <div class="title">
      <setting-config theme="two-tone" size="24" :fill="['#efefef', '#00000020']" />
      <span>技能特长</span>
    </div>
    <div class="skillbox">
      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #ff0066 0%, #ff00cc 100%); width: 80%"
        >
          <span>Java</span>
        </div>
        <div class="skill-bar-percent">80%</div>
      </div>
      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #ffb7dd 0%, #ffb7dd 100%); width: 80%"
        >
          <span>SpringBoot</span>
        </div>
        <div class="skill-bar-percent">80%</div>
      </div>
      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #00bcd4 0%, #80deea 100%); width: 70%"
        >
          <span>SpringCloud</span>
        </div>
        <div class="skill-bar-percent">70%</div>
      </div>
      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #ffeb3b 0%, #fff176 100%); width: 70%"
        >
          <span>Linux</span>
        </div>
        <div class="skill-bar-percent">70%</div>
      </div>
      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #4caf50 0%, #81c784 100%); width: 60%"
        >
          <span>Mybatis/MybatisPlus</span>
        </div>
        <div class="skill-bar-percent">60%</div>
      </div>
      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #ffeb3b 0%, #CCFF99 100%); width: 50%"
        >
          <span>mongodb</span>
        </div>
        <div class="skill-bar-percent">50%</div>
      </div>

      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #ffeb3b 0%, #FF5511 100%); width: 50%"
        >
          <span>redis</span>
        </div>
        <div class="skill-bar-percent">50%</div>
      </div>

      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #9900ff 0%, #cc66ff 100%); width: 40%"
        >
          <span>vue</span>
        </div>
        <div class="skill-bar-percent">40%</div>
      </div>

      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #33FFFF 0%, #9955FF 100%); width: 40%"
        >
          <span>Nginx</span>
        </div>
        <div class="skill-bar-percent">40%</div>
      </div>

      <div class="skillbar">
        <div
          class="skillbar-title"
          style="background: linear-gradient(to right, #5500DD 0%, #7A0099 100%); width: 30%"
        >
          <span>RabbitMq</span>
        </div>
        <div class="skill-bar-percent">30%</div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { mainStore } from "@/store";
import { SettingConfig } from "@icon-park/vue-next";
const store = mainStore();
onMounted(() => {});

onBeforeUnmount(() => {});
</script>

<style lang="scss" scoped>
.time-capsule {
  width: 100%;
  .title {
    display: flex;
    flex-direction: row;
    align-items: center;
    margin: 0.2rem 0 1.5rem;
    font-size: 1.1rem;
    .i-icon {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-right: 6px;
    }
  }
  .text {
    display: block;
    margin: 1rem 0rem 0.5rem 0rem;
    font-size: 0.95rem;
  }

  .skillbar {
    position: relative;
    display: block;
    max-width: 360px;
    margin: 15px 10px;
    background: #eee;
    height: 30px;
    border-radius: 35px;
    -moz-border-radius: 35px;
    -webkit-border-radius: 35px;
    -webkit-transition: 0.4s linear;
    -moz-transition: 0.4s linear;
    -o-transition: 0.4s linear;
    transition: 0.4s linear;
    -webkit-transition-property: width, background-color;
    -moz-transition-property: width, background-color;
    -o-transition-property: width, background-color;
    transition-property: width, background-color;
  }

  .skillbar .skillbar-title {
    position: absolute;
    top: 0;
    left: 0;
    width: 110px;
    font-size: 0.9rem;
    color: #ffffff;
    border-radius: 35px;
    -webkit-border-radius: 35px;
    -moz-border-radius: 35px;
  }
  .skillbar .skillbar-title span {
    display: block;
    background: rgba(0, 0, 0, 0.15);
    padding: 0 20px;
    height: 30px;
    line-height: 30px;
    border-radius: 35px;
    -webkit-border-radius: 35px;
    -moz-border-radius: 35px;
  }
  .skillbar .skill-bar-percent {
    position: absolute;
    right: 10px;
    top: 0;
    font-size: 12px;
    height: 30px;
    line-height: 30px;
    color: #ffffff;
    color: rgba(0, 0, 0, 0.5);
  }
}
</style>
