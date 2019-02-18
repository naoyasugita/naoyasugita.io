<template>
  <div>
    <ul>
      <li v-for="(tab, index) in tabs" :key=index>
         <router-link v-bind:to=tab.path>
            {{ tab.title }}
         </router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'MainHeader',
  data () {
    return {
      tabs: [
        { title: 'TOP', path: '/' },
        { title: 'PROFILE', path: '/profile' },
        { title: 'SKILL', path: '/Skill' },
      ]
    }
  }
}
</script>

<style scoped>
ul {
  margin: auto;
  width: 480px;
  display:flex;
  justify-content: center;
  padding: 10px;
  list-style: none;
}

li {
  width: 120px;
  height: 50px;
  margin-left:20px;
  margin-right:20px;
  position: relative;
}

li:hover {
  opacity: 0.4;
}

a {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  text-decoration: none;
  line-height: 50px;
  font-size:30px;
  color:black;
}
</style>