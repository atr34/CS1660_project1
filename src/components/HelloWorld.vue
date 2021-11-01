<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h3>
      Welcome to Big Data Processing Application. Please type the number that corresponds to which application you would like to run
    </h3>
    <ul>
      <li>
        <a
          href="https://localhost:8888"
          target="_blank"
          rel="noopener"
          >Jupyter Notebook</a
        >
      </li>
      <li>
        <a
          href="https://www.google.com/search?q=surprised+pikachu&tbm=isch&source=iu&ictx=1&fir=6Z68SObMlC4mNM%252CpiImvZWPel5uTM%252C_%253BgKZj2KqNs3j7iM%252C5YcvXlvmJKa0mM%252C_%253BkfzAmIvnLfn2eM%252CpiImvZWPel5uTM%252C_%253B2yNR_1VHIL7-JM%252CW-ZAvKsV9QxEQM%252C_%253BOlC7GKEeY4pC3M%252CYbPtvIpsxdDCsM%252C_%253BWx0PJHGWFF4w8M%252CcEshfimaJ2ReyM%252C_%253BdzEphZEuTaaDPM%252CRByOGimA700NyM%252C_%253BTX-zDEkfvJ4K8M%252Cu0NhJuexf-pDPM%252C_%253BI74hSEO_wd-BlM%252CW-ZAvKsV9QxEQM%252C_%253Bai6Hrhu4QZa2rM%252CTC5YfA499T_uUM%252C_%253BTwHvPMHeOQVZ5M%252C3kxi4p8neOFaaM%252C_%253BLs4U_9Qzi55knM%252CGKiOSo0MBlIcvM%252C_%253BjJ4Y1yrcSj71qM%252CwpWoMefL1FxYMM%252C_%253BYTT61zl-_2hc9M%252C_EqJ28FgOoaPdM%252C_&vet=1&usg=AI4_-kS7WSHZNYTX9j2jY-LVBJqrAj0g6w&sa=X&ved=2ahUKEwiQiZXqkfbzAhVFYTUKHTr5C3kQ9QF6BAgEEAE#imgrc=6Z68SObMlC4mNM"
          target="_blank"
          rel="noopener"
          >Apache Hadoop</a
        >
      </li>
      <li>
        <a
          href="https://localhost:8081"
          target="_blank"
          rel="noopener"
          >Apache Spark</a
        >
      </li>
      <li>
        <a
          href="https://localhost:8082"
          target="_blank"
          rel="noopener"
          >SonarQube and SonnarScanner</a
        >
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
