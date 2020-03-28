<template>
  <div class="hm-credit-card">
    <div class="container">
      <div class="header">
        <div class="avatar">
          <text class="avatarText">{{ options.avatarText }}</text>
        </div>
        <div class="person">
          <div class="name">
            <text class="nameText">{{ options.nameText }}</text>
            <image class="nameIcon" :src="options.nameIcon" />
          </div>
          <text class="introduce">{{ options.introduce }}</text>
        </div>
      </div>
      <div class="main">
        <div class="backgourdLine"><div class="pointLine" /></div>
      </div>
      <div class="bottom">
        <text class="curriculum">{{ options.curriculum }}</text>
        <text class="points">{{ options.points }}</text>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmCreditCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-credit-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          avatarText: '王',
          nameText: '王小二',
          nameIcon:
            './images/img_24428_0_0.png',
          introduce: '介绍',
          curriculum: '课程',
          points: '79分'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>
