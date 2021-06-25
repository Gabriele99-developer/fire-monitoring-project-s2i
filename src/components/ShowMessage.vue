<template>
  <div>
    <h1>
      <span v-for="(letter, index) in title" :key="index" class="letter">{{ letter }}</span>
    </h1>
    <h2>{{ message }}</h2>
  </div>

</template>

<script>
import '@/assets/styles/ShowMessage.scss'
export default {
  name: 'ShowMessage',
  props: ['message', 'title']
}
</script>
