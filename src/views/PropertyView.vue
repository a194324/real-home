<template>
  <MainContainer>
    <PropertyKg :properData="properData"/>
    <Nov2Kg :propenData="propenData"/>
    <Nov3Kg :propevData="propevData"/>
    <PaginationKg/>
  </MainContainer>
</template>

<script>
import {propevData} from '../data/data.dummy'
import {propenData} from '../data/data.dummy'
import {properData} from '../data/data.dummy'

import MainContainer from '../components/MainContainer';
import PropertyKg from  '../components/PropertyKg'
import Nov2Kg from  '../components/Nov2Kg'
import Nov3Kg from  '../components/Nov3Kg'
import PaginationKg from  '../components/PaginationKg'

export default {
  name: 'PropertyView',
  components: {
  MainContainer,
  PropertyKg,
  Nov2Kg,
  Nov3Kg,
  PaginationKg,

  },
  data() {
    return {
      properData: properData,
      propenData: propenData,
      propevData: propevData,


    }
  }
}
</script>

