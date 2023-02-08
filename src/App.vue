<template>
  <ul>
    <LearningResource v-for="res in storedResources" :key="res.id" />
  </ul>
</template>

<script>
import LearningResource from './components/learning-resources/LearningResource.vue';

export default {
  components: {
    LearningResource,
  },
  data() {
    return {
      storedResources: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official documentation of Vue',
          link: 'https://vuejs.org',
        },
        {
          id: 'google',
          title: 'Google',
          description: 'Learn how to Google..',
          link: 'https://google.com',
        },
      ],
    };
  },
};
</script>
