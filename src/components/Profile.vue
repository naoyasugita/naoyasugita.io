<template>
  <div class="all">
    <main-header />
    <div v-for="(article, index) in articles" :key="index">
      <div class="article">
        <div v-if="article.subject !== 'Interset'">
          <h1>{{ article.subject }}</h1>
          <table>
            <tr v-for="(value, key, index) in article.value" :key="index">
              <td>{{ key }}</td>
              <td>{{ value }}</td>
            </tr>
          </table>
        </div>
        <div v-else class="interset">
          <h1>{{ article.subject }}</h1>
          <p v-for="(val, index) in article.value" :key="index">{{ val }}</p>
        </div>
      </div>
    </div>
    <sns />
  </div>
</template>

<script>
import MainHeader from "./MainHeader";
import Sns from "./Sns";
export default {
  name: "Profile",
  components: {
    MainHeader,
    Sns
  },
  data() {
    return {
      name: "Profile",
      articles: [
        {
          subject: "Profile",
          value: {
            Name: "Naoya Sugita",
            Age: 22,
            Sex: "Male",
            Regides: "Miyazaki"
          }
        },
        {
          subject: "Career",
          value: {
            "H.S.": "West of Miyazaki",
            "Univ.": "Sojo University",
            "Co.": "aratana inc."
          }
        },
        {
          subject: "Interset",
          value: [
            "Python",
            "Machine Learning",
            "Web",
            "Outdoor",
            "Animation",
            "etc..."
          ]
        }
      ]
    };
  }
};
</script>
<style scoped>
.all {
  margin: 0px;
  font-size: 30px;
}
h1,
h2 {
  font-size: 50px;
  font-weight: bold;
  margin: 10px;
}
table {
  margin: auto;
}
th,
td {
  padding: 0px 10px;
}
.subject {
  color: red;
}
.interset p {
  margin-top: 0px;
  margin-bottom: 0px;
}
.footer {
}
</style>
