<template>
  <div class="hello">
    <main-header />
    <h2>Level</h2>
    <p>novice : learned in class or only tutorial</p>
    <p>intermediate : Available levels with reference</p>
    <p>advanced : vailable levels can be used on a daily basis</p>
    <div>
      <div class="content">
        <h1>Languages</h1>
        <h2>novice</h2>
        <img src="../../static/skill/c.svg" width="48" />
        <img src="../../static/skill/c++.svg" width="48" />
        <img src="../../static/skill/java.svg" width="48" />
        <h2>intermediate</h2>
        <img src="../../static/skill/html5.svg" width="48" />
        <img src="../../static/skill/css3.svg" width="48" />
        <img src="../../static/skill/javascript.svg" width="48" />
        <img src="../../static/skill/php.svg" width="48" />
        <img src="../../static/skill/mysql.svg" width="48" />
        <h2>advanced</h2>
        <img src="../../static/skill/python.svg" width="48" />
      </div>

      <div class="content">
        <h1>Framework</h1>
        <h2>novice</h2>
        <img src="../../static/skill/django.svg" width="48" />
        <img src="../../static/skill/laravel.svg" width="48" />
        <h2>intermediate</h2>
        <img src="../../static/skill/flask.svg" width="48" />
        <img src="../../static/skill/vue-dot-js.svg" width="48" />
        <h2>advanced</h2>-
      </div>

      <div class="content">
        <h1>Tools/OS</h1>
        <h2>novice</h2>
        <img src="../../static/skill/docker.svg" width="48" />
        <img src="../../static/skill/webpack.svg" width="48" />
        <img src="../../static/skill/heroku.svg" width="48" />
        <img src="../../static/skill/firebase.svg" width="48" />
        <h2>intermediate</h2>
        <img src="../../static/skill/slack.svg" width="48" />
        <img src="../../static/skill/git.svg" width="48" />
        <img src="../../static/skill/github.svg" width="48" />
        <img src="../../static/skill/jupyter.svg" width="48" />
        <img src="../../static/skill/tensorflow.svg" width="48" />
        <img src="../../static/skill/linux.svg" width="48" />
        <img src="../../static/skill/apple.svg" width="48" />
        <img src="../../static/skill/windows.svg" width="48" />
        <h2>advanced</h2>-
      </div>

      <div class="content">
        <h1>Other</h1>
        <img src="../../static/skill/visualstudiocode.svg" width="48" />
        <img src="../../static/skill/kaggle.svg" width="48" />
        <img src="../../static/skill/raspberry-pi.svg" width="48" />
      </div>
    </div>
  </div>
</template>

<script>
import MainHeader from "./MainHeader";
export default {
  name: "Top",
  components: {
    MainHeader
  },
  data() {
    return {
      name: "Skill"
    };
  }
};
</script>

<style scoped>
h1,
h2 {
  font-weight: bold;
}
.content {
  width: 500px;
  display: inline-block;
  vertical-align: top;
  margin: 15px 0px;
  padding: 10px;
}
img {
  padding: 5px;
}
p {
  font-size: 20px;
}
</style>
