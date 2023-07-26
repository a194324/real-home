<template>
  <div class="row">
    <div class="col-md-3 col-sm-12" v-for="property in propevData" :key="property.id">
      <div class="properties__col">
        <img :src="require(`../assets/images/nov3/${property.image}.png`)" :alt="property.desc.sqft"
          class="properties__img img-fluid" />
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
</template>
<script>
export default {
  props: {
    propevData: {
      type: Array,
      default: () => [],
    },
  },
}
</script>