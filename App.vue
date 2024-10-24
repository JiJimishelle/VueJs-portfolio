<template>
  <div class="header">
    <li><router-link to="/"><img src="./assets/logo.png"> </router-link></li>
  </div>
  <div id ="index" > 
    <div id="container">
      <div id ="nav">
        <ul class="menu">
          <li> <a href="#">나의 소개</a> 
            <ul class="submenu">
              <li><router-link to="/resume"> 이력서 </router-link></li>
              <li><router-link to="/selfintro"> 자기 소개서 </router-link></li>
            </ul>
          </li>

          <li>
          <a href="#">자격증</a>
            <ul class="submenu">
              <li><router-link to="/certificate1"> 가천대 성적증명서</router-link></li>
              <li><router-link to="/certificate2"> 몽골국립대학교 공자학원 </router-link></li>
              <li><router-link to="/certificate3"> 유학생 시간제취업 허가 </router-link></li>
              <li><router-link to="/certificate4"> MIA 심사원 증면서</router-link></li>
              <li><router-link to="/certificate5"> 한국어 능력시험</router-link></li>
              <li><router-link to="/certificate6"> 중국어 능력시험</router-link></li>
            </ul>
          </li>

          <li>
          <a href="#">과외 활동</a>
            <ul class="submenu">
              <li><router-link to="/contest1"> 댄스 활동  </router-link></li>
              <li><router-link to="/contest2"> 아르바이트 </router-link></li>
              <li><router-link to="/contest3"> 일본 애니  </router-link></li>
            </ul>
          </li>

          <li>
          <a href="#">진로</a>
            <ul class="submenu">
              <li><router-link to="/career1"> 자연언어처리 개념 </router-link></li>
              <li><router-link to="/career2"> NLP 작업</router-link></li>
              <li><router-link to="/career3"> 제가 개발하고자 하는 부분</router-link></li>
            </ul>
          </li>
        </ul>
      </div>
      <br/><br/>
      <div id = "main">
        <router-view/> 
      </div>
     </div>  
    
    <footer>
      Copyright 2024. Galbadrakh Misheel all rights reserved.
      <br/>
      연락처 : 010-8089-6215
    </footer>
  </div>  
</template>

<style src="./App.css">
</style>