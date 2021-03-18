<template>
 <div class="contact">
     <p>Contact Us</p>
     <ul>
         <li>
             Email: Vue@edu.vn
         </li>
         <li>
             Phone: +84123456789
         </li>
     </ul>
 </div>
</template>

<script>
export default {
    data() {
        return {

        };
    },
    mounted(){
        console.log('Create')
    },
    beforeUnmounted(){
        console.log('ready to destroy')
    },
    unmounted() {
    console.log('Destroyed!!1');
  },
  deactivated(){
      console.log('Deactive!!!')
  },
  activated(){
      console.log('Actived!')
  },
  beforeUpdate() {
      console.log('123321')
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>