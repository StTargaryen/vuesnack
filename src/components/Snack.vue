<template>
  <div class="fixed w-full top-0 left-0 flex justify-center mt-6">
    <transition name="snack">
      <div
        class="bg-blue-500 text-white px-8 py-2 rounded-lg text-sm"
        v-if="snack"
      >
        {{ snack }}
      </div>
    </transition>
  </div>
</template>

<script>
import { mapGetters } from "vuex";
export default {
  computed: {
    ...mapGetters({
      snack: "snack",
    }),
  },
};
</script>

<style lang="scss" scoped>
</style>