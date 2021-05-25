<template>
  <div class="app-section dark row">
      <div class="col-12 app-section-title-wrapper">
        <div class="app-section-title light">Testimonies</div>
      </div>
      <app-testimony v-for="(testimony, index) in testimonies" :key="index"
            :text="testimony.text"
            :name="testimony.name"
            :role="testimony.role"
        />
  </div>
</template>

<script>
  import appTestimony from "../Testimony";
  export default {
    data(){
      return{
        testimonies: [
            { text: 'This initiate supported our health workers in all ways possible', role: 'Head of SouthGate', name: '-Sarah Finhead' },
            { text: 'This initiate supported our health workers in all ways possible', role: 'Head of SouthGate', name: '-Sarah Finhead' },
            { text: 'This initiate supported our health workers in all ways possible', role: 'Head of SouthGate', name: '-Sarah Finhead' }
        ]
      }
    },
    components: {
        appTestimony
    }
  }
</script>

<style>
  
</style>