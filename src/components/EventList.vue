<template>
  <div class="event-list">
    <div class="event-list__content">
      <button class="event-list__content__button">
        <img src="../assets/icons/arrow_left_white.svg" alt="Seta apontando para direita" />
      </button>
      <h2 class="event-list__content__title">Programação</h2>
      <ul class="event-list__content__card-list">
        <li><EventCard></EventCard></li>
        <li><EventCard></EventCard></li>
        <li><EventCard></EventCard></li>
        <li><EventCard></EventCard></li>
        <li><EventCard></EventCard></li>
        <li><EventCard></EventCard></li>
      </ul>
    </div>
  </div>
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
.event-list {
  background-color: rgba(4, 33, 73, 0.9);
  font-family: "Montserrat", sans-serif;
  height: 100vh;
  display: flex;
}

.event-list__content {
  margin: 0 0 40px 0;
  padding: 40px;
  text-align: left;
  overflow-y: auto;
  white-space: nowrap;
}

button {
  background: transparent;
  border: none;
  cursor: pointer;

  img {
    width: 40px;
  }
}

h2 {
  font-size: 40px;
  text-transform: uppercase;
  font-weight: bold;
  margin: 20px 0 0 0;
}

ul, li {
  margin-top: 0;
  padding: 0;
  list-style-type: none;
}
</style>
