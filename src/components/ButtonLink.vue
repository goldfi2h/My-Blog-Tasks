<template>
    <div v-for="item in listItems" :key="item.id">
        <button 
        class="btn btn-link"
        >{{item.title}}</button>
      </div>
</template>

<script setup>
import { ref } from 'vue';
const listItems = ref([]);

async function getData() {
  const res = await fetch("http://my-fire.test/api/blog");
  const finalRes = await res.json();
  listItems.value = finalRes;
}

getData()
</script>

<script>
    export default{
        name: 'ButtonLink',
        props: {
            text: String,
        },
        methods: {
            onClick(){
                this.$emit('btn-click')
            }
        }
    }
</script>