<template>
  <div class="hello">
    <h1>Ola Norman</h1>
    <img
      src="https://media.licdn.com/dms/image/C4E03AQFuI-9ceWkKoA/profile-displayphoto-shrink_200_200/0?e=1553126400&v=beta&t=ml21h12q2Owvl-2vywvuHjcs3rWvwCFw0h65YLZQfZY"
      height="150"
      width="150"
    >
    <CVArea header="Erfaringer" title="Amazon" subTitle="CEO" text="Beste CEO Amazon har hatt"/>
    <CVArea header="Verv" title="MC Donalds" subTitle="Servicearbeider" text="Årets ansatt 7 år på rad"/>
    <CVArea header="Utdanning" title="NTNU" subTitle="Fulgetitter" text="Ekspert på fulger"/>
  </div>
</template>

<script>
import CVArea from "./CVArea.vue";

export default {
  name: "CV",
  components: {
    CVArea
  },
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  width: 60%;
  align-self: center;
}

img {
  border-radius: 50%;
}

h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
