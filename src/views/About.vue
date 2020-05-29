<template>
  <div class="about">
    <agile :initial-slide="3">
      <div class="slide">
        <iframe
          style="border: 0; width: 350px; height: 588px;"
          src="https://bandcamp.com/EmbeddedPlayer/album=3450742190/size=large/bgcol=ffffff/linkcol=0687f5/transparent=true/"
          seamless
        >
          <a
            href="http://elihpoehtrecord.bandcamp.com/album/without-words"
          >Without words by ELIHPOEHT records</a>
        </iframe>
      </div>
      <div class="slide">
        <iframe
          style="border: 0; width: 350px; height: 588px;"
          src="https://bandcamp.com/EmbeddedPlayer/album=1066367559/size=large/bgcol=ffffff/linkcol=0687f5/transparent=true/"
          seamless
        >
          <a href="http://elihpoehtrecord.bandcamp.com/album/power">Power by ELIHPOEHT records</a>
        </iframe>
      </div>
      <div class="slide">
        <iframe
          style="border: 0; width: 350px; height: 720px;"
          src="https://bandcamp.com/EmbeddedPlayer/album=2896597964/size=large/bgcol=ffffff/linkcol=0687f5/transparent=true/"
          seamless
        >
          <a
            href="http://elihpoehtrecord.bandcamp.com/album/relovution"
          >Relovution by ELIHPOEHT records</a>
        </iframe>
      </div>
      <div class="slide">
        <iframe
          style="border: 0; width: 350px; height: 522px;"
          src="https://bandcamp.com/EmbeddedPlayer/album=1465202985/size=large/bgcol=ffffff/linkcol=0687f5/transparent=true/"
          seamless
        >
          <a
            href="http://elihpoehtrecord.bandcamp.com/album/sad-morning"
          >Sad morning by ELIHPOEHT records</a>
        </iframe>
      </div>
      <div class="slide">
        <iframe
          style="border: 0; width: 350px; height: 654px;"
          src="https://bandcamp.com/EmbeddedPlayer/album=4292621044/size=large/bgcol=ffffff/linkcol=0687f5/transparent=true/"
          seamless
        >
          <a href="http://elihpoehtrecord.bandcamp.com/album/memories">Memories by ELIHPOEHT records</a>
        </iframe>
      </div>
      <div class="slide">
        <iframe
          style="border: 0; width: 350px; height: 786px;"
          src="https://bandcamp.com/EmbeddedPlayer/album=3263780869/size=large/bgcol=ffffff/linkcol=0687f5/transparent=true/"
          seamless
        >
          <a
            href="http://elihpoehtrecord.bandcamp.com/album/samples-from-the-sun"
          >Samples from the sun by ELIHPOEHT records</a>
        </iframe>
      </div>
      <template slot="prevButton">
        <i class="fas fa-chevron-left"></i>
      </template>
      <template slot="nextButton">
        <i class="fas fa-chevron-right"></i>
      </template>
    </agile>
  </div>
</template>

<script>
import { VueAgile } from "vue-agile";
export default {
  components: {
    agile: VueAgile
  },
  data() {
    return {};
  }
};
</script>

<style scoped>
.agile__nav-button {
  background: transparent;
  border: none;
  color: #fff;
  cursor: pointer;
  font-size: 24px;
  height: 100%;
  position: absolute;
  top: 0;
  -webkit-transition-duration: 0.3s;
  transition-duration: 0.3s;
  width: 80px;
}
.agile__nav-button:hover {
  background-color: rgba(0, 0, 0, 0.5);
  opacity: 1;
}
.agile__nav-button--prev {
  left: 0;
}
.agile__nav-button--next {
  right: 0;
}
.agile__dots {
  bottom: 10px;
  left: 50%;
  position: absolute;
  -webkit-transform: translateX(-50%);
  transform: translateX(-50%);
}
.agile__dot {
  margin: 0 10px;
}
.agile__dot button {
  background-color: transparent;
  border: 1px solid #fff;
  border-radius: 50%;
  cursor: pointer;
  display: block;
  height: 10px;
  font-size: 0;
  line-height: 0;
  margin: 0;
  padding: 0;
  -webkit-transition-duration: 0.3s;
  transition-duration: 0.3s;
  width: 10px;
}
.agile__dot--current button,
.agile__dot:hover button {
  background-color: #fff;
}

.slide {
  display: block;
  height: 500px;
  -o-object-fit: cover;
  object-fit: cover;
  width: 100%;
}
</style>
