<template>
  <li>
    <h3>{{ topicName }}</h3>
    <p>{{ description }}</p>
    <button @click="selectTopicMy(id)">Learn More</button>
  </li>
</template>

<script>
export default {

  inject:['selectTopicMy'],
  props: ['id', 'topicName', 'description'],
  emits: ['select-topic'],
};
</script>