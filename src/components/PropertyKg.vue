<template>
<div class="property-views">
<div class="property-view">
  <h1 class="property-catalog">Property <b>Catalog</b></h1>
  </div>
<nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container container-main">
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav navbar-property">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">
              CHICAGO
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">KANSAS CITY</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">DENVER</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">NEW-YORK</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">LONDON</a>
          </li>
        </ul>
    </div>
    </div>
  </nav>
<div class="row">
          <div class="col-md-6 col-sm-12" v-for="property in properData" :key="property.id">
            <div class="properties__col">
              <img :src="require(`../assets/images/pro/${property.image}.jpg`)" :alt="property.desc.sqft"
                class="properties__img" />
              <h4 class="properties__h4">{{ `${property.desc.sqft} ${property.title}` }}</h4>
              <p class="properties__sub">{{ property.subtitle }}</p>
              <p class="properties__price">${{ property.price }}</p>
              <ul class="properties__desc">
                <li class="properties__item">{{ property.desc.sqft }} Sq Ft</li>
                <li class="properties__item">{{ property.rooms }} Bedrooms</li>
                <li class="properties__item">{{ property.bath }} Bathroom</li>
              </ul>
            </div>
          </div>
        </div>
        </div>
        </template>
        <script>
        export default {
          props: {
            properData: {
              type: Array,
              default: () => [],
            },
          },
        }
        </script>

        <style lang="scss">
        .property-catalog {
          font-family: Raleway;
          font-size: 45px;
          line-height: 50px;
          font-weight: 300;
          color: #3c3c3c;
          font-weight: 500;
        }
        .container-main{
          max-width: 1550px;
          padding: 50px 60px;
        }
        .navbar-property{
          margin-bottom: 100px;
        }

        .navbar-property li{

          padding:50px 30px;
          font-family: Raleway;
          font-size: 20px;
          line-height: 60px;
          font-weight: 700;
          color: #3c3c3c;
          color: #797979;
        }
</style>