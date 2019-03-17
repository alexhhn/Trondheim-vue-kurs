<template>
  <div class="cvArea">
    <h2>{{header}}</h2>
    <div class="content-container">
      <h3>{{title}}</h3>
      <h4>{{subTitle}}</h4>
      <p>{{text}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "CVArea",
  props: {
    header: String,
    title: String,
    subTitle: String,
    text: String
  }
};
</script>

<style scoped>
.cvArea {
  display: flex;
  flex-direction: column;
}

h2 {
  align-self: flex-start;
  font-size: 16px;
  margin: 0;
  margin-bottom: 5px;
}

h4 {
  font-weight: normal;
}

p {
  font-size: 14px;
  font-weight: 300;
}

h3,
h4,
p {
  margin: 0;
  margin-bottom: 5px;
}

.content-container {
  background-color: white;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 15px;
  margin-bottom: 20px;
}
</style>
