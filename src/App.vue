<template>
  <h2>My Course Goal</h2>
  <!-- Task 1: Output your main course goal with help of the composition API -->
  <!-- Don't hardcode it into the template, instead hardcode it into the JS code -->
  <h3 v-if="toggle">{{ goal }}</h3>
  <!-- Task 2: Toggle (show/ hide) the goal with help of the button  -->
  <button @click="switchGoal">Toggle Goal</button>
  <!-- Task 3: Manage data in three ways -->
  <!-- => Separate refs -->
  <!-- => Ref Object -->
  <!-- => Reactive Object -->
  <!-- Task 4: Also solve the assignment with the Options API -->
</template>

<script>
// import { ref } from 'vue';
// import { reactive } from 'vue';

export default {
  // setup() {
  //   // const goal = ref('Success');
  //   // const toggle = ref(true);

  //   // const info = ref({
  //   //   goal: 'Success',
  //   //   toggle: true,
  //   // });

  //   const info = reactive({
  //     goal: 'Success',
  //     toggle: true,
  //   });

  //   function switchGoal() {
  //     // toggle.value = !toggle.value;
  //     // info.value.toggle = !info.value.toggle;
  //     info.toggle = !info.toggle;
  //   }

  //   return { info, switchGoal };
  // },

  data() {
    return {
      goal: 'Success',
      toggle: true,
    };
  },

  methods: {
    switchGoal() {
      this.toggle = !this.toggle;
    },
  },
};
</script>

<style>
html {
  font-family: sans-serif;
}
body {
  margin: 3rem;
  text-align: center;
}
</style>