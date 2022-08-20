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
const route = useRoute()
const id = Number(route.params.id)
const fishdata = data.find(res=>res.id === id)
</script>
<template>
<div class="container mt-5">
    <div class="card" style="width: 18rem;">
        <div class="card-header">
            名称：{{ fishdata.name }}
        </div>
        <ul class="list-group list-group-flush">
            <li class="list-group-item">生息地：{{fishdata.place}}</li>
            <li class="list-group-item">旬：{{fishdata.season}}</li>
        </ul>
    </div>
    <Nuxt-link to="/fishdata">back</Nuxt-link>
</div>
</template>