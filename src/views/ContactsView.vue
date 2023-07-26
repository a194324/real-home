<template>
  <div class="contact-view">
    <ContactKg/>


    <ContactKg2/>
  </div>
</template>
<script>
import ContactKg from '../components/ContactKg'
import ContactKg2 from '../components/ContactKg2'

export default {
  name: 'ContactsView',
  components:{
 ContactKg,
 ContactKg2,
  },
  data() {
    return {




    }
  }
}
</script>