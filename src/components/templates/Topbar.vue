<template>
  <div class="top-bar">
    <div class="profile-section" v-if="chat.value">
      <div class="text-wrapper">
        <p>{{ chat.value.from }}</p>
        <span class="type">
          <a>{{ chat.value.email }}</a>
        </span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["chat"]
};
</script>
