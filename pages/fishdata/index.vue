<script setup>
const data = [
    {
        "id": 1,
        "name": "メバル",
        "place": "北海道南部～九州の沿岸部",
        "season": "春から冬",
    },
    {
        "id": 2,
        "name": "アジ",
        "place": "全国各地",
        "season": "初夏から晩夏",
    },
    {
        "id": 3,
        "name": "カサゴ",
        "place": "日本近海～太平洋西部",
        "season": "冬から春",
    },
]
</script>
<template>
<div>
    <h1>fish data</h1>
    <div v-for="value in data">
    <Nuxt-link :to='"/fishdata/"+value.id'> {{ value.name }}</Nuxt-link>
    </div>
</div>
</template>