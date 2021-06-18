<template>
    <div class="container" style="margin-top:15vh">
        <div class="row justify-content-center">
          <div class="col-12 col-lg-9">
          <h3>卷積神經網路擴增實境遮蔽感知系統(Convolutional Neural Network Augmented Reality Occlusion-aware System)</h3>
          <hr>
          <p>
            當今主流的擴增實境應用是Apple，搭載光達來掃描場景物體深度，本論文完全不依靠硬體設備的協助，使用深度學習模型估算光流，改進現有技術的不穩定性，完全以軟體計算場景深度，完成擴增實境的沈浸式體驗。
          </p>
          <p><img class="mx-auto d-block" style="max-width:400px" src="../assets/img/paper1.png" alt=""></p>
          <h3>系統介紹</h3> 
          <hr>
          <p>本論文所提的系統分為 6 大步驟。第一步驟為計算序列影幀光流。第二步驟為計算光流梯度與原影幀梯度。第三步驟為融合光流梯度與原始影像梯度產生軟深度邊緣。第四步驟為修改 Canny Edge 獲得定位準確的邊緣圖。第五步驟為產生稀疏點雲資訊。最後一個步驟為將稀疏點雲資訊傳播至定位準確的邊緣圖中，產生深度圖。
</p>
          <p><img class="mx-auto d-block" style="max-width:400px" src="../assets/img/paper2.png" alt=""></p>

            <h3>擴增實境效果製作流程</h3>
            <p><img class="mx-auto d-block" style="max-width:400px" src="../assets/img/paper3.png" alt=""></p>
            <p>首先將手機拍 攝的影片輸入 Adobe 特效軟體 After Effect，使用 After Effect 特效功能中的 3D 相機追 蹤功能，還原手機鏡頭移動軌跡。第二步將還原的相機軌跡連動至 Autodesk 的 3D 動畫 製作軟體，將欲加入了真實場景中的虛擬物體放入相機場景中，再輸出成具有色彩的 3D 物件影片以及 3D 物件深度圖影片。也將手機拍攝的影片輸入深度圖系統至中，產生場 景深度圖影片。最後再使用 OpenCV 與本深度圖系統的深度圖做結合，產生具有擴增實 境遮蔽感知效果的影片。</p>
          </div>
        </div>
    </div>
</template>