<template>
  <layout class-prefix="layout">
    <NumberPad/>
    <Types/>
    <Notes/>
    <Tags :data-source.sync="tags"/>
  </layout>
</template>
<style lang="scss">
  .layout-content {
    display: flex;
    flex-direction: column-reverse;
  }
</style>


<script>
  import NumberPad from '@/components/NumberPad'
  import Types from '@/components/Types'
  import Notes from '@/components/Notes'
  import Tags from '@/components/Tags'
  export default {
    name: 'Money',
    components: {Tags, Notes, Types, NumberPad},
    data(){
      return{
        tags:['衣','食','住','行']
      }
    }

  }
</script>

