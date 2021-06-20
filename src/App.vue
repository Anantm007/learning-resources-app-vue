<template>
<LearningResource v-for="res in storedResources" :key="res.id" />
  <ul></ul>
</template>

<script>
import LearningResource from './components/learning-resources/LearningResource.vue';

export default {
  components: {LearningResource};
  data() {
    return {
      storedResources: [
        {
          id: '1',
          title: 'Official Guide',
          description: 'This is the official Vue js doc',
          link: 'https://vuejs.org'
        },
        {
          id: '2',
          title: 'Google',
          description: 'This is the official google doc',
          link: 'https://google.com'
        }
      ]
    };
  }
};
</script>
