<template>
  <div>
    <main-header />
    <img src="../../static/top.png" />
  </div>
</template>

<script>
import MainHeader from "./MainHeader";
import Sns from "./Sns";
export default {
  name: "Top",
  components: {
    MainHeader
  },
  data() {
    return {
      name: "Top"
    };
  }
};
</script>
<style scoped>
h1,
h2 {
  font-weight: normal;
}
img {
  width: 100vw;
}
</style>
