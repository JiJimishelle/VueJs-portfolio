<template>
  <div class="contest">
    <fieldset>
      <legend>댄스 활동</legend>
      고급 교육을 받는 것도 중요하지만, 동아리, 스포츠, 과외 활동에 참여하는 
      것이 다재다능한 학생이 되는 데 도움이 된다고 생각합니다. 그럼으로, 어렸을 때부터 
      여러가지 활동에 참여해 왔습니다.
    </fieldset>
    <div class="image-container">
      <img src="../assets/dance.png" alt="dance"/>
      <img src="../assets/dance2.png" alt="dance"/>
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
