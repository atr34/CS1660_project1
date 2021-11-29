<template>
  <div class="Dashboard">
    <h1 class="subheading grey--text text-center">Select the Big Data Tool you wish to use</h1>
    <v-container class="my-5">
      <v-card flat color="grey lighten-4" class="pa-3">
        <v-row wrap>
          <v-col cols="6">
            <div class="caption grey--text">Service</div>
            <div class="caption">Jupyter Notebook</div>
          </v-col>
          <v-col cols="2">
            <div class="caption grey--text">Person</div>
            <div class="caption">Aaron Reuter</div>
          </v-col>
          <v-col cols="2">
            <div class="caption grey--text">Url</div>
            <div class="caption">
              <input
                type="button"
                onclick="window.open('http://35.237.237.196:8888/','_blank','resizable=yes')"
                value="Jupyter Notebook"
              />
            </div>
          </v-col>
        </v-row>
      </v-card>
      <br />
      <v-card flat color="grey lighten-4" class="pa-3">
        <v-row wrap>
          <v-col cols="6">
            <div class="caption grey--text">Service</div>
            <div class="caption">Apache Hadoop</div>
          </v-col>
          <v-col cols="2">
            <div class="caption grey--text">Person</div>
            <div class="caption">Aaron Reuter</div>
          </v-col>
          <v-col cols="2">
            <div class="caption grey--text">Url</div>
            <div class="caption">
              <input
                type="button"
                onclick="window.open('http://34.73.165.139:9870/','_blank','resizable=yes')"
                value="Apache Hadoop"
              />
            </div>
          </v-col>
        </v-row>
      </v-card>
      <br />
      <v-card flat color="grey lighten-4" class="pa-3">
        <v-row wrap>
          <v-col cols="6">
            <div class="caption grey--text">Service</div>
            <div class="caption">Apache Spark</div>
          </v-col>
          <v-col cols="2">
            <div class="caption grey--text">Person</div>
            <div class="caption">Aaron Reuter</div>
          </v-col>
          <v-col cols="2">
            <div class="caption grey--text">Url</div>
            <div class="caption">
              <input
                type="button"
                onclick="window.open('http://35.227.51.22:8080/','_blank','resizable=yes')"
                value="Apache Spark"
              />
            </div>
          </v-col>
        </v-row>
      </v-card>
      <br />
      <v-card flat color="grey lighten-4" class="pa-3">
        <v-row wrap>
          <v-col cols="6">
            <div class="caption grey--text">Service</div>
            <div class="caption">SonarQube and SonarScanner</div>
          </v-col>
          <v-col cols="2">
            <div class="caption grey--text">Person</div>
            <div class="caption">Aaron Reuter</div>
          </v-col>
          <v-col cols="2">
            <div class="caption grey--text">Url</div>
            <div class="caption">
              <input
                type="button"
                onclick="window.open('http://34.139.16.186:9000/','_blank','resizable=yes')"
                value="SonarQube and SonarScanner"
              />
            </div>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>
