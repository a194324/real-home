<template>
<div class="blog">
    <div class="container">
      <div class="row">
        <div class="col-md-8 col-sm-12" v-for="blog in blogData" :key="blog.id">
          <div class="blog__col ">
            <h2 class="blog__title">{{ blog.title }}</h2>
            <img class="blog__img" :src="require(`../assets/images/blog/${blog.image}.png`)" :alt="blog.title" />
            <p class="blog__p">{{ blog.text }}</p>
            <button type="button" class="btn btn-danger">Read More</button>
          </div>
        </div>
        <div class="col-md-4 col-sm-12">
          <div class="categories__col">
            <h2>Categories</h2>
            <a href="#">Art Directionn</a>
            <a href="#">Digital Photography</a>
            <a href="#">Information Architecture</a>
            <a href="#">Interior Design</a>
            <a href="#">Photoshop Tools</a>
            <a href="#">Mosion Grafics</a>
          </div>
          <div class="arhives__col">
             <h2>Arhives</h2>
            <a href="#">May 2014</a>
              <a href="#">March 2013</a>
              <a href="#">February 2013</a>
              <a href="#">January 2013</a>
              <a href="#">December 2012</a>
              <a href="#">May 2012</a>
          </div>
        </div>
      </div>
    </div>
  </div>





</template>
<script>
export default {
  props: {
    blogData: {
      type: Array,
      default: () => [],
    },
  },
}
</script>
<style lang="scss">
.categories__col{
  position: absolute;
  top: 120px;
  right:200px ;
width: 187px;
height: 226px;

  display: block;
  &>a{
text-decoration: none;
font-family: Raleway;
font-size: 18px;
line-height: 35px;
font-weight: 500;
color: #797979;

  }
}
.blog__col{
  margin-bottom: 50px;
}
.arhives__col{
   position: absolute;
  top: 520px;
  right:200px ;
width: 187px;
height: 226px;
&>a{
text-decoration: none;
font-family: Raleway;
font-size: 18px;
line-height: 35px;
font-weight: 500;
color: #797979;
}
}
.blog__p{
  margin-bottom: 30px;
  width: 724px;
  height: 93px;
  font-family: 'Playfair Display';
font-size: 16px;
line-height: 27px;
font-weight: 400;
color: #797979;
}
.blog__img{
  margin-bottom: 40px;
}
</style>
