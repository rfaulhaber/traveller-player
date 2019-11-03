<template>
  <div class="button-box">
    <button>1D</button>
    <button>2D</button>

    <div v-if="currentCharacter">your name is: {{currentCharacter.name}}</div>
  </div>
</template>

<script>
export default {
  name: "Roller",
  props: {
    currentCharacter: Object
  }
};
</script>

<style scoped>
.button-box {
  border: 1px solid black;
}
</style>