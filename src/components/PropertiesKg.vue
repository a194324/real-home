<template>
  <div class="properties">
    <MainContainer>
      <div class="row">
        <div class="col">
          <h2 class="properties__h2">
            Featured
            <b>Properties</b>
          </h2>
        </div>
        <div class="col">
          <p class="properties__subtitle">
            Quisque diam lorem interdum vitaapibus vitae pede. Donec eget tellus non erat lacinia fertum. Donec in velit
            vel ipsum auctovinar.
          </p>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4 col-sm-12" v-for="property in propertiesData" :key="property.id">
          <div class="properties__col">
            <img :src="require(`../assets/images/${property.image}.png`)" :alt="property.desc.sqft"
              class="properties__img" />
            <h4 class="properties__h4">{{ `${property.desc.sqft} ${property.title}` }}</h4>
            <p class="properties__sub">{{ property.subtitle }}</p>
            <p class="properties__price">{{ property.price }}</p>
            <ul class="properties__desc">
              <li class="properties__item">{{ property.desc.sqft }} Sq Ft</li>
              <li class="properties__item">{{ property.rooms }} Bedrooms</li>
              <li class="properties__item">{{ property.bath }} Bathroom</li>
            </ul>
          </div>
        </div>
      </div>
    </MainContainer>
  </div>
</template>

<script>
import MainContainer from './MainContainer.vue';

export default {
    props: {
        propertiesData: {
            type: Array,
            default: () => [],
        },
    },
    components: { MainContainer }
}
</script>
