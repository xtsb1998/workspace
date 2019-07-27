<template>
  <section class="main">
    <button2></button2>
    <button1></button1>
    <button3></button3>
    <button4></button4>
  </section>
</template>

<script>
import button1 from "./button/button";
import button2 from "./button/buttonA";
import button3 from "./button/buttonB";
import button4 from "./button/buttonC";
export default {
  data() {
    return {
      visible: false
    };
  },
  components: {
    button1,button2,button3,button4
  }
};
</script>

