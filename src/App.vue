<template>
  <div id="app">
    <!-- <movable
      posTop="2022"
      posLeft="30"
      class="modaltitle movable-img"
      target="parentEl"
    >
      <img src="@/assets/channels/presentation.png" alt="" />
    </movable>

    <movable
      posTop="800"
      posLeft="1090"
      class="modaltitle movable-img"
      target="parentEl"
    >
      <img src="@/assets/channels/internet.png" alt="" />
    </movable> -->

    <!-- <div
      class="channel"
      v-for="(channelName, index) in channels"
      :key="channelName"
    >
      <movable
        :posTop="positions[index][1]"
        :posLeft="positions[index][0]"
        class="modaltitle movable-img"
        target="parentEl"
      >
        <img :src="require('@/assets/channels/' + channelName + '.png')" />
      </movable>
    </div> -->

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
      <h1 class="large">
        {{ titleOptions[titleIndex] }}
      </h1>
    </section>

    <section>
      <img src="@/assets/presentationofself.jpeg" alt="" />
      <p>"The world, in truth, is a wedding."</p>
    </section>
    <aside>❋</aside>
    <section>
      <!-- <img src="@/assets/tbh.png" alt="" /> -->
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
    <!-- <aside>❋</aside>
    <section>
      <img src="@/assets/trickmirror.jpeg" alt="" />
      <p>
        "You can’t just walk around and be visible on the internet--for anyone
        to see you, you have to <i>act</i>."
      </p>
    </section> -->
    <aside>❋</aside>
    <section>
      <h1>Putting myself on screen</h1>
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
          src="@/assets/777_final_compressed.mp4"
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

    <!-- <section>
      <img
        src="https://images-na.ssl-images-amazon.com/images/I/918FaSUn+mL.jpg"
        alt=""
      />
      <p>
        "A woman must continually watch herself. She is almost continually
        accompanied by her own image of herself."
      </p>
    </section>
    <aside>❋</aside> -->
    <section>
      <h1>Putting myself on screen some more!!!</h1>

      <article>
        <p><i>Glance Back</i></p>
        <p>
          You spend so much time looking at your computer... doesn't your
          computer deserve a chance to look back at you?
        </p>

        <img src="@/assets/1_question.png" alt="" />
        <img src="@/assets/2_mainpage.png" alt="" />
        <p>
          Glance Back is a daily photo diary, capturing the moments shared
          between you and your computer.
        </p>
        <video
          autoplay
          loop
          muted
          playsinline
          src="@/assets/glancebacks_2021-09-28.mp4"
        ></video>
        <img src="@/assets/glancebackchromeweb.png" alt="" />
        <video
          autoplay
          loop
          muted
          playsinline
          src="https://glanceback.info/assets/gallery/Sal.mp4"
        ></video>

        <video
          autoplay
          loop
          muted
          playsinline
          src="https://glanceback.info/assets/gallery/LaurenGlanceBack.mp4"
        ></video>
      </article>
      <article>
        <p><i>THE MODEL MINORITY IS A MYTH!</i></p>
        <iframe
          src="https://www.are.na/maya-man/gospel-billboards"
          frameborder="0"
        ></iframe>
        <img
          src="https://mayaontheinter.net/media/pages/index/projects/the-model-minority-is-a-myth/07df52ee12-1626825609/2_maya_edit.jpg"
          alt=""
        />
        <img
          src="https://mayaontheinter.net/media/pages/index/projects/the-model-minority-is-a-myth/8320a587cc-1626825609/4_tweet.png"
          alt=""
        />
      </article>
    </section>
    <aside>❋</aside>
    <section>
      <p>Okay so where am I going with this?</p>

      <div class="channels">
        <div
          class="channel"
          v-for="channelName in channels"
          v-bind:key="channelName"
        >
          <img :src="require('@/assets/channels/' + channelName + '.png')" />
        </div>
      </div>
      <article>
        <iframe src="https://whoisjadeontheinter.net/" frameborder="0"></iframe>
      </article>

      <iframe
        width="200"
        height="315"
        src="https://www.youtube.com/embed/PMxECpwMesQ"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
      <img src="@/assets/comment_01.png" alt="" />
      <img src="@/assets/comment_02.jpg" alt="" />
      <img src="@/assets/comment_03.jpg" alt="" />
      <img src="@/assets/comment_04.jpg" alt="" />

      <!-- <article>
        <a
          data-pin-do="embedBoard"
          data-pin-board-width="900"
          data-pin-scale-height="500"
          data-pin-scale-width="800"
          href="https://www.pinterest.com/mayaontheinternet/quotes/"
        ></a>
      </article> -->
      <aside>❋</aside>

      <h1>Thanks for listening : - )</h1>
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
      channels: [
        "presentation",
        "girlhood",
        "girlboss",
        "influencerburnout",
        "tiktok",
        "cyber",
        "bigbeauty",
        "work",
        "womxnartists",
      ],
      channelArchive: [
        "buyingthings",
        "internet",
        "collaging",
        "fastfashion",
        "website",
      ],
      positions: [
        [50, 1194],
        [1090, 2389],
        [35, 3582],
        [1119, 4776],
        [50, 5970],
        [1090, 7164],
        [75, 8358],
        [1119, 9552],
        [50, 10746],
        [1090, 11940],
        [35, 13134],
        [1119, 14328],
        [100, 15522],
        [1090, 16716],
        [35, 17910],
        [1119, 19104],
      ],
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
  /* background: url("https://media.istockphoto.com/photos/light-blue-spring-sky-picture-id466951264?k=20&m=466951264&s=612x612&w=0&h=r6J9dhGuLW4GRzPicUQAaRPSpz0qStcdFYJwJb040BY=");
  background-position: center center;
  background-repeat: no-repeat;
  background-size: 100% 100%; */
  /* background: rgb(255, 204, 255); */
  background: #cbe3ff;
  /* background: #d0e8f1; */
  /* background: #e6dac1; */
  /* background: blue; */
}

.movable-img {
  display: block;
  margin: auto;
  width: 200px;
  height: auto;
}

h1,
h2,
h3,
h4,
h5,
p,
a,
iframe,
img,
video {
  padding: 0;
  margin: 25px 0px;
  max-width: 100%;
  width: 100%;
}

iframe {
  margin: auto;
  display: block;
  height: 500px;
}

#app {
  /* font-family: "Crimson Text", serif; */
  /* font-family: Arial, Helvetica, sans-serif; */
  font-family: serif;
  font-size: 48px;
  line-height: 72px;
  font-weight: normal;
  text-align: center;
  color: #ed1288;

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  margin-top: 60px;
  width: 60%;
  margin: auto;
}

a {
  color: #ed1288;
  font-style: italic;
}

a:hover {
  color: blue;
  cursor: alias;
}

.clickable:hover {
  color: blue;
  cursor: pointer;
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
  color: blue;
}

h1,
.large {
  /* font-size: 108px;
  line-height: 140px; */
  font-weight: normal;
  font-size: 48px;
  line-height: 72px;
  /* padding: 0px; */
  /* margin: 0px; */
}

.regular {
}

::selection {
  background: blue;
}

section {
  margin: 50px 0;
}

article {
  padding: 50px 0px;
}

.channels {
  display: flex;
  /* flex-flow: row; */
  /* flex-flow: wrap; */
  justify-content: space-around;
  flex-wrap: wrap;
}

.channel {
  max-width: 30%;
}
</style>
