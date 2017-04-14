<template>
  <div class="hello">
    <editor v-model="code"></editor>
    <preview v-model="code" debounce="500"></preview>
  </div>
</template>

<script>
import Editor from '@/components/editor'
import Preview from '@/components/preview'
export default {
  name: 'hello',
  components: {
    Editor,
    Preview
  },
  data () {
    return {
      code: `
<md-button class="md-raised md-primary">Hello</md-button>
<md-button class="md-raised md-warn">Hello</md-button>
`
    }
  }
}
</script>
