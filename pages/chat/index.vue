<template>
  <view class="chat">
    <view class="send">
      <tn-input
        placeholder="请输入内容"
        border="surround"
        v-model="problem"
      ></tn-input>
      <tn-button
        iconColor="#ffffff"
        color="#26B3A0"
        text="发送"
        @tap="getAnswer"
      >
      </tn-button>
    </view>
  </view>
</template>

<script>
import chatMixin from "../../mixins/chat.js";
export default {
  mixins: [chatMixin],
  data() {
    return {
      type: "chat",
    };
  },
};
</script>

<style lang="scss" scoped>

</style>
