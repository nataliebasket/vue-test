<script>
export default {
    props: {
        name: String,
        color: String,
        price: Number,
        count: Number,
    },
    data() {
    return {
        flowersCounter: this.count
    }
  }
}
</script>

<template>
    <article>
        <h3>{{ name }}</h3>
        <p>Цвет: {{ color }}</p>
        <p>Цена: {{ price }}р/шт</p>
        <p>Количество <input type="number" min="1" name="count" v-model="flowersCounter"></p>
        <p>Итого: {{( price * flowersCounter)}} за 1 шт</p>
        <button type="button">Добавить в корзину</button>
    </article>
</template>