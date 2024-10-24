<template>
  <div class="contest">
    <fieldset>
      <legend>일본 애니</legend>
      중학교 때부터 애니를 좋아하게 되었으며, 일어로 어떤 말을 하든 진절하게 들려서
      본어를 독학으로 배우게 되었습니다.
    </fieldset>
    <div class="image-container">
      <img src="../assets/anime.png" alt="dance"/>
      <img src="../assets/anime2.png" alt="dance"/>
    </div>
  </div>
</template>

<style scoped>
  .image-container {
    display: flex;
    justify-content: space-around; 
    align-items: center; 
    margin-top: 30px;
  }
  img {
    max-width: 45%; 
  }
  legend{
    color: white;
    font-size: 28px;
    font-weight: 530;
  }
</style>
