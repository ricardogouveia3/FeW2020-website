<template>
  <ul class="event-list__content__card-list">
    <li><EventCard></EventCard></li>
    <li><EventCard></EventCard></li>
    <li><EventCard></EventCard></li>
    <li><EventCard></EventCard></li>
    <li><EventCard></EventCard></li>
    <li><EventCard></EventCard></li>
  </ul>
</template>

<script>
import EventCard from './EventCard.vue';

export default {
  name: 'EventList',
  components: {
    EventCard,
  },
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  ul {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
    grid-gap: 15px;
    margin-top: 50px;
    padding: 0;
  }

  li {
    list-style-type: none;
  }
</style>
