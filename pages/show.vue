<template>
    <div>
        <items></items>
    </div>
</template>

<script>
    import Items from '~/components/items.vue'

    export default {
      components: {
        Items
      },
      async fetch ({ store }) {
        await store.dispatch('LOAD_ITEMS', 'showstories.json')
      }
    }
</script>