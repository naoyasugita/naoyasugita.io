<template>
  <div>
    <main-header/>
    <img src="../../static/top_img.jpg">
    <sns/>
  </div>
</template>

<script>
import MainHeader from './MainHeader'
import Sns from './Sns'
export default {
  name: 'Top',
  components: {
    MainHeader,
    Sns
  },
  data () {
    return {
      name:'Top',
    }
  },
}
</script>
<style scoped>
h1, h2 {
  font-weight: normal;
}
img {
	width: 100vw;
}
</style>
