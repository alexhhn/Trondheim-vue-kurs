<template>
  <div class="hello">
    <img :src="avatar" height="150" width="150">
    <h1>Ola Norman</h1>
    <p>IT Konsulent</p>

    <div v-for="area in areas" :key="area.id">
      <CVArea
        :header="area.header"
        :title="area.title"
        :subTitle="area.subTitle"
        :text="area.text"
      />
    </div>
  </div>
</template>

<script>
import CVArea from "./CVArea.vue";
import Pic from "@/assets/ola.jpeg";
export default {
  name: "CV",
  data() {
    return {
      avatar: Pic,
      areas: [
        {
          id: 1,
          header: "Erfaringer",
          title: "Amazon",
          subTitle: "CEO",
          text: "Beste CEO Amazon har hatt"
        },
        {
          id: 2,
          header: "Verv",
          title: "MC Donalds",
          subTitle: "Servicearbeider",
          text: "Årets ansatt 7 år på rad"
        },
        {
          id: 3,
          header: "Utdannning",
          title: "NTNU",
          ubTitle: "Fulgetitter",
          text: "Ekspert på fulger"
        }
      ]
    };
  },
  components: {
    CVArea
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  width: 60%;
}

h1 {
  margin: 10px 0;
}

p {
  margin: 5px 0 10px 0;
}
img {
  border-radius: 50%;
}

h3 {
  margin: 40px 0 0;
}

a {
  color: #42b983;
}
</style>
