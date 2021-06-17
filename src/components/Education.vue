<template>
<!-- work eperience -->

  <div class="container">
    <h3>工作經驗</h3>
    <hr>
    <ul class="sessions lstyle">
      <li class="list lstyle">
      <div class="time"><a style="text-decoration: none;" href="https://hiero7.com/">禾新數位有限公司</a> RD暑期實習生 (2018年7月～2018年8月)</div>
        <p>工作內容</p>
        <ul type="disc">
          <li><p>使用Python開發自動化爬蟲報表產生系統，幫助公司減少大量人力及時間</p></li>
          <li><p>將公司網站更改為使用 Vue CLI 進行維護與修改，串接 Google Analytics 和 Boomerang 進行網站分析，以及套用 Vue I18n 增加多國語言功能</p></li>
        </ul>		
      </li>
    </ul>		
  </div>

<!-- work experience -->

<div class="container">
  <h3>學歷</h3>
  <hr>	
</div>

<div class="container">
  <div class="wrapper">
  <!-- <h1> 國立臺北科技大學資訊工程學系研究所, 2019年9月 ～ 2021年1月</h1> -->
    <ul class="sessions lstyle">
      <li class="list lstyle">
      <div class="time">國立臺北科技大學資訊工程學系研究所, 2019年9月 ～ 2021年1月</div>
      <ul type="disc">
        <li><p>參加 PRAGMA 37 研討會 獲得<a style="text-decoration: none;" href="file:///Users/wupinyi/Downloads/student-awards.pdf">最佳海報第一名</a></p></li>
        <li><p>擔任 計算機程式語言助教(c語言)</p></li>
        <li><p>擔任 電資外國學生專班計算機程式設計助教(c語言)</p></li>
        <li><p>擔任 基礎程式設計助教(HTML,CSS,JQuery,JavaScript,reavel.js,SVG)</p></li>
        <li><p>擔任 離散數學助教</p></li>
        <li><p>擔任 109科技部計畫研究助理，負責「機器學習遮蔽感知擴增實境」之計畫書撰寫及研究開發</p></li>
        <li><p>擔任 110科技部計畫研究助理，負責「機器學習」之計畫書撰寫</p></li>
        <li><p>擔任 無人車計畫研究助理,負責同時定位與地圖構建(SLAM)之研究</p></li>
        <li><p>參與 馬來西亞多媒體大學(MMU)共同開發Hubot機器人應用功能</p></li>
        <li><p>設計開發 臺北科技大學、西門子和中正高中AI學程簽訂記者會之開幕Hubot機器人表演</p></li>		
        <li><p>碩士論文:<a style="text-decoration: none;" href="https://hdl.handle.net/11296/mqn85y">卷積神經網路擴增實境遮蔽感知系統</a></p></li>
      </ul>
      </li>
      <li class="list lstyle">
      <div class="time">國立臺北科技大學資訊工程學系, 2015年9月 ～ 2019年6月</div>
        <ul type="disc">
          <li><p>資訊工程系系學會總務長，並擔任多項系上活動幹部，參與舉辦兩屆資工營(霍格華資的逆襲，星際資戰)</p></li>
          <li><p>實務專題競賽佳作:<a style="text-decoration: none;" href="https://csie.ntut.edu.tw/csie/Chinese/06Students/data/107/107_project_award.html">客製化大眾交通之旅客資訊顯示屏</a></p></li>
        </ul>
      </li>
    </ul>
  </div>
</div> 
</template>

<script>
export default {
}
</script>

<style scoped>

.lstyle{
  list-style: none;
  padding: 0;
}

.sessions {
  margin-top: 2rem;
  border-radius: 12px;
  position: relative;
}

.list {
  padding-bottom: 1.5rem;
  border-left: 1px solid #abaaed;
  position: relative;
  padding-left: 20px;
  margin-left: 10px;
}
.list:last-child {
  border: 0px;
  padding-bottom: 0;
}
.list:before {
  content: "";
  width: 15px;
  height: 15px;
  background: white;
  border: 1px solid #4e5ed3;
  box-shadow: 3px 3px 0px #bab5f8;
  box-shadow: 3px 3px 0px #bab5f8;
  border-radius: 50%;
  position: absolute;
  left: -10px;
  top: 0px;
}

.time {
  color: #2a2839;
  font-family: "Poppins", sans-serif;
  font-weight: 500;
}
@media screen and (min-width: 601px) {
  .time {
    font-size: 1.05rem;
  }
}
@media screen and (max-width: 600px) {
  .time {
    margin-bottom: 0.3rem;
    font-size: 1rem;
  }
}

p {
  color: #4f4f4f;
  font-family: sans-serif;
  line-height: 1.5;
  margin-top: 0.4rem;
}
@media screen and (max-width: 600px) {
  p {
    font-size: 1.05rem;
  }
}
</style>