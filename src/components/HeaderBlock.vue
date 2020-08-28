<template>
  <v-card>

  </v-card>
</template>

<script>
export default {
  name: "HeaderBlock",
  data() {
    return {
      tab: null,
      navItems: [
        {
          title: 'ГЛАВНАЯ',
          href: '#main'
        }, {
          title: 'ОБУЧЕНИЕ',
          href: '#education'
        }, {
          title: 'РАБОТА',
          href: '#work'
        }, {
          title: 'НАВЫКИ',
          href: '#skills'
        }
      ],
    }
  }
}
</script>

<style scoped>

</style>