<template>
  <a 
    :href="'http://' + link" 
    target="_blank" 
    rel="noopener noreferrer"
  >
    <slot/>
  </a>
</template>

<script>
export default {
  props: {
    link: {type: String, required: true}
  }
}
</script>
