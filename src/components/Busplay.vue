<template>
    <div class="container" style="margin-top:15vh">
        <div class="row justify-content-center">
          <div class="col-12 col-lg-9">
          <h3>Busplay (Bus+display)</h3>
          <hr>
          <p>
            這是一套放置在車內的資訊顯示系統，可以讓業者製作每一條路線，客製化每站站點的資訊，並根據情境設定投放廣告圖片，提供三大功能給乘客：路線資訊、周邊介紹及廣播投放。
          </p>
          <p><img class="mx-auto d-block" style="max-width:400px" src="../assets/img/busplay1.png" alt=""></p>
          <p>顯⽰屏幕提供三⼤功能：路線資訊、周邊介紹和廣播投放。路線資訊不僅顯⽰最重要的站點與預估到站時間，還提供了即時天氣資訊與跑⾺燈⽂字，可 ⽤於配合政府政策宣導；周邊介紹功能推薦站點附近景點、商圈和美⾷資訊等；廣播投放可放置圖⽚與影⽚，⽤於配合政府活動宣傳或商家商品推廣。 後台系統提供多語⾔輸⼊選單、路線主題⾊挑選、公⾞路線匯⼊功能、站點資訊編輯與廣播觸發情境設定。匯集民眾意⾒並彌補現有顯⽰器不⾜處，將其改善並整合於後台調整。</p>
          <h3>介面</h3> 
          <hr>
          <p class="text-center"> 
            <figure class="mb-4">
            <img class="mx-auto d-block" style="max-width:400px" src="../assets/img/busplay2.png" alt="">
            <figcaption>▲周邊介紹</figcaption>
            </figure>
            <figure class="mb-4">
            <img class="mx-auto d-block" style="max-width:400px" src="../assets/img/busplay3.png" alt="">
            <figcaption>▲廣播投放</figcaption>
            </figure>
            <figure class="mb-4">
            <img class="mx-auto d-block" style="max-width:400px" src="../assets/img/busplay4.png" alt="">
            <figcaption>▲路線選擇</figcaption>
            </figure>
            <figure class="mb-4">
            <img class="mx-auto d-block" style="max-width:400px" src="../assets/img/busplay5.png" alt="">
            <figcaption>▲後台管理</figcaption>
            </figure>
            <!-- <figure class="mb-4">
            <img class="mx-auto d-block" style="max-width:400px" src="../assets/img/busplay6.png" alt="">
            <figcaption>▲系統架構圖</figcaption>
            </figure> -->
          </p>
          <h3>系統架構</h3> 
          <hr>
          <p><img class="mx-auto d-block" style="max-width:400px" src="../assets/img/busplay6.png" alt=""></p>
          <p>利⽤ MongoDB 作為 Database、NodeJS 作為伺服器，透過 REST 架構作為主要取得資料⽅式。依據新北市、台北市資料開放平台 API，解析後取得實⽤路線與站點資訊存進資料庫。最後藉由 Google Maps API 與 Here Map API 圖資運算出道路距離與取得天氣狀況，交由前端顯⽰屏幕顯⽰。</p>
          </div>
        </div>
    </div>
</template>