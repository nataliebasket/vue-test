<script>
import CardFlower from './CardFlower.vue'

export default {
  components: {
    CardFlower
  },
  data() {
    return {
        flowers: [
            {
                name: 'Тюльпан',
                color: 'Белый',
                price: 1300,
                count: 1,
            },
            {
                name: 'Роза',
                color: 'Красный',
                price: 1200,
                count: 1,
            },
            {
                name: 'Василек',
                color: 'Синий',
                price: 1500,
                count: 3,
            },
        ]
    }
  }
}
</script>

<template>
    <h2>Каталог цветов</h2>
    <section>
        <template v-for="flower in flowers">
            <!-- <CardFlower :name="flower.name" :color="flower.color"
             :price="flower.price" :count="flower.count" /> -->
             <CardFlower v-bind="flower"/>
        </template>
    </section>
</template>

<style scoped>
section {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;

}
</style>
