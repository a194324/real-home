<template>
  <MainContainer>
    <div class="about-view">
<div class="about__title">
  <h2>About Our Company</h2>
</div>
<div class="row">
  <div class="col-lg-8 col-md-12 col-sm-12">
    <img src="../assets/images/about/about_1.jpg" alt="">
  </div>
  <div class="col-lg-4 col-md-12 col-sm-12">
    <p class="textkg">Quisque diam lorem interdum vitaapibus ac scelerisque vitae pede. Donec eget tellus non erat lacinia fertum. Donec in velit vel ipsum auctovinar. Proin umcorper urna et felisstibulum iaculis lacinia est. Proin dictum elem entum velit fusce euismod. Aenean commodo ligula eget dolor. Aenean massa. Lorem ipsum dolor sit amet, consec tetuer adipis elit, aliquam eget nibh etlibura. Lorem ipsum dolor sitamet, consetetur sadipscing elitr.Quisque diam lorem interdum vitaapibus ac scelerisque vitae pede. Donec eget tellus non erat lacinia fertum. Donec in velit vel ipsum auctovinar.  </p>
  </div>
</div>
  </div>
  <FeautersKg :data="featureData" />
  <PropertiesKg :propertiesData="propertiesData" />
  <OurTeam :propertiesData="propertiesData"/>
  <OurrKg :quData="quData"/>
  <SubscribeBanner/>
  </MainContainer>

</template>
<script>
import { featureData,propertiesData,quData} from '../data/data.dummy'
import MainContainer from '../components/MainContainer';
import FeautersKg from '../components/FeautersKg';
import PropertiesKg from '../components/PropertiesKg';
import OurTeam from '../components/OurTeam'
import OurrKg from '../components/OurrKg'
import SubscribeBanner from '../components/SubscribeBanner'


export default {
  name: 'aboutView',
  components: {
    MainContainer,
    FeautersKg,
    PropertiesKg,
    OurTeam,
    OurrKg,
    SubscribeBanner,

  },
  data() {
    return {
      featureData: featureData,
      propertiesData: propertiesData,
       quData: quData,






    }
  }
}
</script>
<style>
.about-view{
  display: block;
align-items: center;
  padding: 10px 100px;
}
.about__title{
font-family: 'Playfair Display';
font-size: 16px;
line-height: 27px;
font-weight: 400;
color: #797979;
}
.textkg{
  font-family: 'Playfair Display';
font-size: 16px;
line-height: 27px;
font-weight: 400;
color: #797979;
}
</style>