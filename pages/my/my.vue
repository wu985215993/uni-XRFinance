<template>
  <view class="header">
    <view class="header__user">
      <view class="header__user__left">
        <image class="header__user__avatar" :src="src"></image>
        <view class="header__user__content">
          <view class="header__user__content__hi">HI 翔瑞用户</view>
          <view class="header__user__content__tags">
            <view class="header__user__content__tag">理财达人</view>
            <view class="header__user__content__tag">未实名 ></view>
          </view>
        </view>
      </view>
      <view class="header__user__right">
        <image class="header__user__right__sign" src="../../static/images/个人/路径 4313@3x.png" mode=""></image>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      src: '../../static/images/个人/椭圆 119@3x.png',
      text: '头像加载失败'
    };
  },
  methods: {}
};
</script>

<style lang="scss" scoped>
.header {
  padding: 38rpx 28rpx 0 0;
  background-color: #3476f1;
  color: #fff;
  &__user {
    display: flex;
    justify-content: space-between;
    &__left{
      display: flex;
    }
    &__avatar {
      width: 84rpx;
      height: 84rpx;
      margin-right: 20rpx;
    }
      
    &__content{
      display: flex;
      flex-direction: column;
      &__hi{
        font-size: 34rpx;
        margin-bottom: 16rpx;
      }
      &__tags{
        display: flex;
      }
      &__tag{
        margin-right: 10rpx;
        text-align: center;
        width: 114rpx;
        font-size: 20rpx;
        line-height: 32rpx;
        border-radius: 32rpx;
        border: 1px solid #fff;;
      }
    }
    &__right{
      &__sign{
        width: 10rpx;
        margin-right: 8rpx;
      }
    }
  }
}
</style>
