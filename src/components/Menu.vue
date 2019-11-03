<template>
  <div>
    <div>
      <Roller v-bind:currentCharacter="character" />
    </div>
    <ul>
      <li>
        <a>Character creation</a>
      </li>
      <li>
        <a>Character sheet</a>
      </li>
    </ul>
  </div>
</template>

<script>
import Roller from "./Roller.vue";

export default {
  name: "Menu",
  components: {
    Roller
  },
  data: function() {
    return {
      character: {
        name: "foo"
      }
    };
  }
};
</script>