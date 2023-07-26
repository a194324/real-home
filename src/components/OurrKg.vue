<template>
  <div class="properties">
    <div class="container">
      <div class="row">
        <div class="col">
          <h2 class="properties__h2">
            НОВЫЙ
            <b>ТОВАР</b>
          </h2>
        </div>
        <div class="col">
          <p class="properties__subtitle">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis ipsa et assumenda neque nostrum placeat
            accusantium minus vel ex, odio, consectetur nam, cupiditate a. Dolore obcaecati veritatis molestiae fugiat
            soluta possimus laborum, quasi repellat sequi totam quibusdam nesciunt aliquam dolor.

          </p>
        </div>
      </div>
      <div class="row">
        <div class="col-md-3 col-sm-12" v-for="about in quData" :key="about.id">
          <div class="properties__col">
            <img :src="require(`../assets/images/our/${about.image}.png`)" :alt="about.title"
              class="properties__img img-fluid" />
            <h4 class="properties__h4">{{ `${about.title}` }}</h4>
            <p class="properties__sub">{{ about.subtitle }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    quData: {
      type: Array,
      default: () => [],
    },
  },
}
</script>
