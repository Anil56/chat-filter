<template>
  <li @click="$emit('click')">
    <div
      class="profile-image"
      style="background-image:url('/images/user1.jpg');"
    ></div>
    <div class="text-wrapper">
      <p>{{ chat.date }}</p>
    </div>
  </li>
</template>

<script>
export default {
  props: ["chat"]
};
</script>
