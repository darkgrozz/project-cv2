<template>
  <div id="c">
    <div v-for="cv in listCv" :key="cv">
      <div id="a">
        <div id="d">
          <h3 id="g" style="margin-top: 50px">
            {{ cv.nama }} <br />
            <font id="e"> {{ cv.nama1 }}</font>
          </h3>
          <img src="gambar.jpg" width="315" height="165" />
          <h3 id="f" v-for="cv in listCv" :key="cv">
            {{ cv.contact }}
          </h3>
          <p id="f">
            <b>{{ cv.judul1 }}</b
            ><br />{{ cv.address }}
          </p>
          <p id="f">
            <b>{{ cv.judul2 }}</b
            ><br />{{ cv.phone }}
          </p>
          <p id="f">
            <b>{{ cv.judul3 }}</b
            ><br /><u>{{ cv.email }}</u>
          </p>
          <p id="f">
            <b>{{ cv.judul4 }}</b
            ><br /><u>{{ cv.link }}</u>
          </p>
          <h3 id="f">
            {{ cv.judul5 }}
            <hr />
          </h3>
          <p id="f">
            {{ cv.bahasa1 }}<br />{{ cv.bahasa2 }}<br />{{ cv.bahasa3 }}
          </p>
          <h3 id="f">
            {{ cv.judul6 }}
            <hr />
          </h3>
          <ul id="f">
            <li>{{ cv.hobi1 }}</li>
            <li>{{ cv.hobi2 }}</li>
            <li>{{ cv.hobi3 }}</li>
            <li>{{ cv.hobi4 }}</li>
          </ul>
        </div>
        <div id="b">
          <h2 style="margin-top: 50px">Summary</h2>
          <hr />
          <p>
            {{ cv.summary }}
          </p>
          <h2>Skill HighLights</h2>
          <hr />
          <div style="display: flex">
            <div>
              <ul>
                <li>{{ cv.skil1 }}</li>
                <li>{{ cv.skil2 }}</li>
                <li>{{ cv.skil3 }}</li>
              </ul>
            </div>
            <ul>
              <li>{{ cv.skil4 }}</li>
              <li>{{ cv.skil5 }}</li>
              <li>{{ cv.skil6 }}</li>
            </ul>
          </div>
          <h2>Experience</h2>
          <hr />
          <p>
            <b>{{ cv.ex1 }}</b
            >{{ cv.ex2 }}<br /><b>{{ cv.ex3 }}</b>
            {{ cv.ex4 }}
          </p>
          <ul>
            <li>
              {{ cv.des1 }}
            </li>
            <li>{{ cv.des2 }}</li>
            <li>
              {{ cv.des3 }}
            </li>
            <li>
              {{ cv.des4 }}
            </li>
          </ul>
          <h2>Education</h2>
          <hr />
          <p>
            {{ cv.edu1 }}<b>{{ cv.edu2 }}</b
            >{{ cv.edu3 }}<br />
            <b>{{ cv.edu4 }}</b> NY
          </p>

          <h2>Certifications</h2>
          <hr />
          <p>
            {{ cv.creative }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CvDua",
  computed: {
    listCv() {
      return this.$store.state.listCv;
    },
  },
};
</script>

<style>
#a {
  display: flex;
  background-color: rgb(189, 189, 189);
}
#b {
  background-color: white;
  padding-left: 10px;
  padding-right: 20px;
  padding-bottom: 100px;
}
#c {
  margin-right: 300px;
  padding-left: 300px;
  margin-top: 50px;
  margin-bottom: 50px;
}
#d {
  font-family: sans-serif;
  padding: auto;
}
#e {
  color: rgb(255, 102, 0);
}
#f {
  margin-right: 20px;
  margin-left: 20px;
}
#g {
  margin-right: 20px;
  margin-left: 20px;
  font-size: 35px;
}
body {
  background-color: gray;
  font-family: sans-serif;
}
</style>