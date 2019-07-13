<template>
  <div id="gallery">
    <ul class="gallery_box">
      <li>
        <a href="#0"><img src="https://picsum.photos/600/700/?random">
          <div class="box_data">
            <span>Ravi With Bike</span>
          </div></a>
      </li>
      <li>
        <a href="#0"><img src="https://picsum.photos/600/701/?random">
          <div class="box_data">
            <span>Ravi Singh</span>
          </div></a>
      </li>
      <li>
        <a href="#0"><img src="https://picsum.photos/600/702/?random">
          <div class="box_data">
            <span>White wall</span>
          </div></a>
      </li>
      <li>
        <a href="#0"><img src="https://picsum.photos/600/703/?random">
          <div class="box_data">
            <span>Green Tree</span>
          </div></a>
      </li>
      <li style="    position: relative;
    top: -134px;">
        <a href="#0"><img src="https://picsum.photos/600/704/?random">
          <div class="box_data">
            <span>Blue</span>
          </div></a>
      </li>
      <li>
        <a href="#0"><img src="https://picsum.photos/600/705/?random">
          <div class="box_data">
            <span>Ravi</span>
          </div></a>
      </li>
    </ul>
  </div>
</template>

<style scoped>
  img{ max-width:100%;}
  .gallery_box li{ width:33.333333%; margin: 0!important; max-width: 100% ; display:inline-block; float: left; text-align: center; overflow: hidden;    position: relative;}
  .gallery_box{ padding:0;display: flow-root;}
  .gallery_box li:hover img {
    -moz-transform: scale(1.1);
    -webkit-transform: scale(1.1);
    -ms-transform: scale(1.1);
    -o-transform: scale(1.1);
    transform: scale(1.1);
  }
  .gallery_box li img{-webkit-transition: transform 0.5s ease;
    -o-transition: transform 0.5s ease;
    transition: transform 0.5s ease;}
  .gallery_box li:nth-child(even) {
    height: 304px;
  }
  .gallery_box li:nth-child(odd) {
    height: 438px;
  }
  .gallery_box li:nth-child(odd) .box_data{ background:rgba(0,0,0,0.17) }
  .gallery_box li:nth-child(even) .box_data{ background:rgba(0,44,255,0.27) }
  .gallery_box .box_data{ position:absolute; top: 0; left: 0; right:0; bottom:0; color:#fff;}
  .gallery_box .box_data span{ position:absolute; top: 50%; transform: translateY(-50%); left:0 ; right:0; font-size:24px;}
  .gallery_box li:hover .box_data{ background:rgba(255,0,39,0.55)}
  @media screen and (max-width: 768px){
    .gallery_box li{
      top: unset!important;
      width: 100%;
      height: auto!important;
    }
  }
</style>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class GalleryBlock extends Vue {
    @Prop() private msg!: string;
}
</script>
