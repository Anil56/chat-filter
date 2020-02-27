<template>
  <div class="chat-scroller">
    <div class="checked" v-if="chat">
      <div class="sent-msg" v-for="(usr, i) in chat" :key="i">
        <div class="text-wrapper">
          <div class="check-flex">
            <div class="text">
              <span>
                {{ usr.msg }}
              </span>
            </div>
          </div>
          <span class="time">{{ usr.time }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["chat"]
};
</script>
