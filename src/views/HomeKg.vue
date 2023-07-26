<template>
  <div class="home">
    <CarouselKg/>
    <MainContainer>
    <div class="row">
      <div class="col-md-4 nome_border">
        <h3 class="home__offeringTitle">We are Offering the
  Best Estate Deals</h3>
      </div>
      <div class="col-md-8">
       <p class="home__paragraf">
  Quisque diam lorem interdum vitaapibus ac scelerisque vitae pede. Donec eget tellus non erat lacinia fertum. Donec in velit vel ipsum auctovinar. Proin umcorper urna et felisstibulum iaculis lacinia est. Proin dictum elem entum velit fusce euismod. Aenean commodo ligula eget dolor. Aenean massa. Lorem ipsum dolor sit amet, consec tetuer adipis elit, aliquam eget nibh etlibura. Lorem ipsum dolor sitamet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et.
       </p>
      </div>
    </div>
    <FeautersKg :data="featureData" />
    <PropertiesKg :propertiesData="propertiesData" />
    </MainContainer>
    <CarouselPictureContent/>
<HomeBanner/>
<CarouselKg2/>
<FotKg/>
  </div>
</template>

<script>
import {featureData,propertiesData} from '../data/data.dummy'

import CarouselKg2 from '../components/CarouselKg2';
import CarouselKg from '../components/CarouselKg';
import FeautersKg from '../components/FeautersKg';
import PropertiesKg from '../components/PropertiesKg';
import CarouselPictureContent from '../components/CarouselPictureContent';
import  HomeBanner from '../components/HomeBanner'
import FotKg from '../components/FotKg';

export default {
  name: 'HomeKg',
  components:{
    CarouselKg,
    CarouselKg2,
    FeautersKg,
    PropertiesKg,
    CarouselPictureContent,
    HomeBanner,
    FotKg,
  },
  data() {
    return {
      featureData: featureData,
      propertiesData: propertiesData,



    }
  }
}
</script>
<style >
</style>