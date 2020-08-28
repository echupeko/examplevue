<template>
  <v-card>

    <v-tabs
        v-model="tab"
        grow
    >
      <v-tab
          v-for="item in items"
          :key="item"
      >
        <v-card :href="item.href">{{ item.title }}</v-card>
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
          v-for="item in items"
          :key="item"
      >
        <v-card
            color="basil"
            flat
        >
          <v-card-text>{{ text }}</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
export default {
  name: "HeaderBlock",
  data() {
    return {
      tab: null,
      items: [
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