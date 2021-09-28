<template>
  <div id="app">
    <!-- <section>
      {{ Math.floor(currentSecond / 60000) }}:{{
        Math.floor(currentSecond / 60000)
      }}
    </section> -->
    <!-- 
    <section>
      <p>Maya Man</p>
    </section> -->

    <section>
      <iframe src="https://mayaontheinter.net/" frameborder="0"></iframe>
      <p>
        <a target="_blank" href="https://mayaontheinter.net/"
          >mayaontheinter.net</a
        >
      </p>
    </section>
    <aside>❋</aside>
    <section>
      <h1 @click="updateTitle()" class="large clickable">
        {{ titleOptions[titleIndex] }}
      </h1>
    </section>

    <section>
      <img src="@/assets/presentationofself.jpeg" alt="" />
      <p>
        "To stay in one's room, away from the place where the party is given is
        to stay away from where reality is being performed. The world, in truth,
        is a wedding."
      </p>
    </section>
    <section>
      <img src="@/assets/trickmirror.jpeg" alt="" />
      <p>
        "You can’t just walk around and be visible on the internet--for anyone
        to see you, you have to <i>act</i>."
      </p>
    </section>

    <aside>❋</aside>
    <section>
      <img src="@/assets/tbh.png" alt="" />
      <video autoplay loop muted playsinline src="@/assets/jazz.mp4"></video>
      <iframe
        width="560"
        height="315"
        src="https://www.youtube.com/embed/kiQFEtm7QYw?start=17"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </section>
    <aside>❋</aside>
    <section>
      <h1>Putting myself on screen (dance, performance, software)</h1>
      <article>
        <video
          autoplay
          loop
          muted
          playsinline
          src="https://mayaontheinter.net/media/pages/index/projects/paint-me-in-pixels/a0da057516-1626825609/paintme_02.mp4"
        ></video>
        <p><i>Paint me in pixels so I can dance forever</i>, (2018)</p>
      </article>
      <article>
        <video
          autoplay
          loop
          muted
          playsinline
          src="https://mayaontheinter.net/media/pages/index/projects/body-movement-language/a9df36824f-1626825609/manifesto_02.mp4"
        ></video>
        <p>
          <i>Body, Movement, Language: A.I. Sketches with Bill T. Jones</i>,
          Google Creative Lab (2019)
        </p>
      </article>

      <article>
        <video
          autoplay
          loop
          muted
          playsinline
          src="@/assets/777_final.mp4"
        ></video>
        <video autoplay loop muted playsinline src="@/assets/joji.mp4"></video>
        <p><i>777 music video for JOJI</i>, directed by Saad Moosajee (2020)</p>
      </article>

      <article>
        <iframe
          src="https://ddsm7s9hd8znk.cloudfront.net/previews/69518c54-2bc5-4b90-b606-675529c7593d/1615845070/index.html#toolbar=0'"
          frameborder="0"
        ></iframe>
        <p><i>can I go where you go?</i>, Feral File (2021)</p>
      </article>
    </section>
    <aside>❋</aside>
    <section>
      <p>Glance Back</p>
      <p>Model Minority Myth</p>
    </section>
    <aside>❋</aside>
    <section>
      <p>Where do I want to go?</p>
      <p>Are.na channels, making sense of TikTok, girlhood, consumerism</p>
      <p>Jade</p>
      <iframe src="https://whoisjadeontheinter.net/" frameborder="0"></iframe>

      <p>Artblocks?</p>
    </section>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      title: "Presentation of self",
      titleOptions: [
        "The presentation of self in everyday life",
        "The presentation of self in everyday life *online*",
      ],
      titleIndex: 0,
      maxSeconds: 600000,
      currentSecond: 600000,
    };
  },
  mounted() {
    // Update the count down every 1 second
    setInterval(() => {
      this.currentSecond--;
    }, 1000);
  },
  methods: {
    updateTitle() {
      this.titleIndex = (this.titleIndex + 1) % this.titleOptions.length;
    },
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Crimson+Text&display=swap");
body {
  background: black;
}

h1,
h2,
h3,
h4,
h5,
p,
a,
iframe {
  padding: 0;
  margin: 25px;
}

#app {
  /* font-family: "Crimson Text", serif; */
  /* font-family: Arial, Helvetica, sans-serif; */
  font-family: serif;
  font-size: 48px;
  line-height: 72px;
  font-weight: normal;
  text-align: center;
  color: white;

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  margin-top: 60px;
  width: 60%;
  margin: auto;
}

a {
  color: white;
  font-style: italic;
}

a:hover {
  color: #ed1288;
  cursor: alias;
}

.clickable:hover {
  color: #ed1288;
  cursor: pointer;
}

img,
video {
  max-width: 100%;
}

iframe {
  max-width: 100%;
  width: 100%;
  margin: auto;
  display: block;
  height: 500px;
}

button {
  margin: 25px;
  padding: 10px;
  background: none;
  border: none;
  font-family: inherit;

  font-size: 48px;
  line-height: 72px;
  font-weight: normal;
  text-align: center;
  color: white;
}

button:hover {
  cursor: pointer;
  color: #ed1288;
}

h1,
.large {
  /* font-size: 108px;
  line-height: 140px; */
  font-weight: normal;
  /* padding: 0px; */
  /* margin: 0px; */
}

.regular {
}

::selection {
  background: #ed1288;
}

section {
  margin: 50px 0;
}

article {
  padding: 50px 0px;
}
</style>
