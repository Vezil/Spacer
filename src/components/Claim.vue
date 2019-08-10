<template>
  <div class="claimWrapper">
    <h1 class="claim">Spacer</h1>
    <p class="subclaim">Begin your journey through our amazin galaxy, and discover places you never even heard of.</p>
    <p class="subclaim">Type anything space-related to start.</p>
  </div>
</template>
<script>
export default {
 name:'Claim',
};
</script>
<style lang="scss" scoped>
  .claimWrapper {
    display:flex;
    flex-direction: column;
    text-align:center;
    justify-content: center;
    align-items: center;
  }

  .claim {
    font-size: 50px;
    margin:0;
      @media(min-width:1024px){
      font-size:80px;
    }
  }

   .subclaim {
    margin: 20px 0 0 0;
    font-size: 13px;
    font-weight:400;


    @media(min-width:768px){
      font-size:17px;
      line-height:1;
      letter-spacing:1px;
      width:500px;
    }
  }

</style>