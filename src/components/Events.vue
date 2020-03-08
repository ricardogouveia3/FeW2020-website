<template>
  <div class="events">
    <div class="events__content">
      <button class="events__content__button">
        <img src="../assets/icons/arrow_left_white.svg" alt="Seta apontando para direita" />
      </button>
      <h2 class="events__content__title">Programação</h2>
      <EventList></EventList>
    </div>
  </div>
</template>

<script>
import EventList from './EventList.vue';

export default {
  name: 'Events',
  components: {
    EventList,
  },
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.events {
  background-color: rgba(4, 33, 73, 0.9);
  font-family: "Montserrat", sans-serif;
  height: 100vh;
  display: flex;

  @media screen and (max-width: 780px) {
    display: none;
  }
}

.events__content {
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
</style>
