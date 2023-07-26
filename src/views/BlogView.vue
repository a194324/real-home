<template>
  <main-container>
  <BlogKg :blogData ="blogData"/>
    <PaginationBlog/>
  </main-container>
</template>

<script>
import MainContainer from '../components/MainContainer';
import { blogData } from '../data/data.dummy'
import BlogKg from '../components/BlogKg';
import PaginationBlog from '../components/PaginationBlog';


export default {
  name: 'HomeKg',
  components: {
BlogKg,
PaginationBlog,
MainContainer,
  },
  data() {
    return {
     blogData: blogData,



    }
  }
}
</script>
<style lang="scss">


</style>