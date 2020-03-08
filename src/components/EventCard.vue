<template>
  <div class="event-card">
    <div class="event-card__header">
      <div class="event-card__header__date">
        <span class="event-card__header__date__day">13</span>
        <div>
          <span class="event-card__header__date__month">Jul</span>
          <span class="event-card__header__date__year">2020</span>
        </div>
      </div>
      <span class="event-card__header__week-day">segunda-feira</span>
    </div>
    <ul class="event-card__events">
      <li>
        <a href="/">
          <div></div>
          <span>JS SP</span>
        </a>
      </li>
      <li>
        <a href="/">
          <div></div>
          <span>CSS SP + Nerdzão</span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'EventCard',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
a { text-decoration: none; }

.event-card {
  background-color: white;
  box-shadow: 0 2px 3px rgba(0, 0, 0, 0.2);
  padding: 30px;
}

ul, li {
  margin: 0;
  padding: 0;
  list-style-type: none;
}

.event-card__header {
  margin-bottom: 20px;
  color: #193058;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.event-card__header__date { display: flex; }

.event-card__header__date div {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.event-card__header__date__day {
  line-height: 1;
  font-weight: bold;
  font-size: 35px;
  margin-right: 5px;
}

.event-card__header__date__month {
  font-size: 13px;
  font-weight: 600;
  text-transform: uppercase;
}

.event-card__header__date__year {
  font-size: 12px;
  font-weight: 400;
  color: #2F59A2;
}

.event-card__header__week-day {
  color: #325798;
  text-align: right;
  text-transform: uppercase;
}

.event-card__events {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;

  li { padding: 5px; }

  li a {
    display: flex;
    align-items: center;
  }

  li div {
    width: 20px;
    height: 20px;
    border-radius: 20px;
    margin-right: 5px;
    background-color: #D8D8D8;
    display: inline-block;
  }

  li span { color: #4A4A4A; }
}
</style>
