<template>
  
<input id="search" name="search" :value="value" :class="{dark}" @input="handleChange"/>
 
</template>
<script>
export default {
 name:'SearchInput',
  props: {
    value: {
      type: String,
      required:true,
    },
    dark: {
      type:Boolean,
      default:false,
    },
  },
  methods: {
    handleChange(e) {
      this.$emit('input', e.target.value);
    },
  },
};
</script>
<style lang="scss" scoped>


  input{
    height: 30px;
    border: 0;
    color:white;
    text-align:center;
    font-size:18px;
    font-weight:300;
    background: none;
    border-bottom: 1px solid white;
    transition: box-shadow .3s ease-out;
    margin-top:3%;

  @media(min-width:1024px){
    font-weight:400;
  }

  }
  input:focus{
    outline:none;
    box-shadow: 0 10px 20px -8px rgba(255,255,255, .5);
  }

.dark{
  color: #1e3d4a;
  border-bottom-color: #1e3d4a;

}

.dark:focus {

box-shadow: 0 10px 20px -8px rgba(#1e3d4a, .5);

}



</style>