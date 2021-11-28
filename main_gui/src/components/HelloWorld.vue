<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h3>
      Please choose the application you would like to run
    </h3>
    <ul>
      <li>
        <input
          type="button"
          onclick="window.open('http://35.237.237.196:8888/','_blank','resizable=yes')"
          value="Jupyter Notebook"
        />
      </li>
      <li>
        <input
          type="button"
          onclick="window.open('http://34.73.165.139:9870/','_blank','resizable=yes')"
          value="Apache Hadoop"
        />
      </li>
      <li>
        <input
          type="button"
          onclick="window.open('http://34.139.16.186:9000/','_blank','resizable=yes')"
          value="Sonar Qube and Sonar Scanner"
        />
      </li>
      <li>
        <input
          type="button"
          onclick="window.open('http://35.227.51.22:8080/','_blank','resizable=yes')"
          value="Apach Spark"
        />
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
</style>
