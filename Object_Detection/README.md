# πμ¬νμ© νλͺ© λΆλ₯λ₯Ό μν Object Detection Reportπ

# λͺ©μ°¨

- [νμκ°](#νμκ°)
- [λν κ°μ](#λν-κ°μ)
- [λ¬Έμ  μ μ](#λ¬Έμ -μ μ)
- [μ€ν λ΄μ©](#λ¬Έμ μ-λν-μ€ν)
- [Modeling λ° Ensemble](#Modeling-λ°-Ensemble)
- [νκ³ ](#νκ³ )

# νμκ°


<table>
  <tr>
    <td align="center">
      <a href="https://github.com/Seoheesu1">
        <img src="https://avatars.githubusercontent.com/u/63832160?v=4" width="100px;" alt=""/>
        <br />
        <sub>μν¬μ</sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/WonsangHwang">
        <img src="https://avatars.githubusercontent.com/u/49892621?v=4" width="100px;" alt=""/>
        <br />
        <sub>ν©μμ</sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/sala0320">
        <img src="https://avatars.githubusercontent.com/u/49435163?v=4" width="100px;" alt=""/>
        <br />
        <sub>μ‘°νμ</sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/hongsusoo">
        <img src="https://avatars.githubusercontent.com/u/77658029?v=4" width="100px;" alt=""/>
        <br />
        <sub>νμν</sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/Junhyuk93">
        <img src="https://avatars.githubusercontent.com/u/61610411?v=4" width="100px;" alt=""/>
        <br />
        <sub>λ°μ€ν</sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/hanlyang0522">
        <img src="https://avatars.githubusercontent.com/u/67934041?v=4" width="100px;" alt=""/>
        <br />
        <sub>λ°λ²μ</sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/GunwooHan">
        <img src="https://avatars.githubusercontent.com/u/76226252?v=4" width="100px;" alt=""/>
        <br />
        <sub>νκ±΄μ°</sub>
      </a>
    </td>
  </tr>
  <tr>
    </td>
  </tr>
</table>
<br>  

# λν κ°μ

![](https://i.imgur.com/PnOdQ0L.png)

λ°μΌνλ‘ λλ μμ°, λλ μλΉμ μλ. μ°λ¦¬λ λ§μ λ¬Όκ±΄μ΄ λλμΌλ‘ μμ°λκ³ , μλΉλλ μλλ₯Ό μ΄κ³  μμ΅λλ€. νμ§λ§ μ΄λ¬ν λ¬Ένλ 'μ°λ κΈ° λλ', 'λ§€λ¦½μ§ λΆμ‘±'κ³Ό κ°μ μ¬λ¬ μ¬ν λ¬Έμ λ₯Ό λ³κ³  μμ΅λλ€.

λΆλ¦¬μκ±°λ μ΄λ¬ν νκ²½ λΆλ΄μ μ€μΌ μ μλ λ°©λ² μ€ νλμλλ€. μ λΆλ¦¬λ°°μΆ λ μ°λ κΈ°λ μμμΌλ‘μ κ°μΉλ₯Ό μΈμ λ°μ μ¬νμ©λμ§λ§, μλͺ» λΆλ¦¬λ°°μΆ λλ©΄ κ·Έλλ‘ νκΈ°λ¬Όλ‘ λΆλ₯λμ΄ λ§€λ¦½ λλ μκ°λκΈ° λλ¬Έμλλ€.

λ°λΌμ μ°λ¦¬λ μ¬μ§μμ μ°λ κΈ°λ₯Ό Detection νλ λͺ¨λΈμ λ§λ€μ΄ μ΄λ¬ν λ¬Έμ μ μ ν΄κ²°ν΄λ³΄κ³ μ ν©λλ€. λ¬Έμ  ν΄κ²°μ μν λ°μ΄ν°μμΌλ‘λ μΌλ° μ°λ κΈ°, νλΌμ€ν±, μ’μ΄, μ λ¦¬ λ± 10 μ’λ₯μ μ°λ κΈ°κ° μ°ν μ¬μ§ λ°μ΄ν°μμ΄ μ κ³΅λ©λλ€.

μ¬λ¬λΆμ μν΄ λ§λ€μ΄μ§ μ°μν μ±λ₯μ λͺ¨λΈμ μ°λ κΈ°μ₯μ μ€μΉλμ΄ μ νν λΆλ¦¬μκ±°λ₯Ό λκ±°λ, μ΄λ¦°μμ΄λ€μ λΆλ¦¬μκ±° κ΅μ‘ λ±μ μ¬μ©λ  μ μμ κ²μλλ€. λΆλ μ§κ΅¬λ₯Ό μκΈ°λ‘λΆν° κ΅¬ν΄μ£ΌμΈμ! π

- **Input :** μ°λ κΈ° κ°μ²΄κ° λ΄κΈ΄ μ΄λ―Έμ§μ bbox μ λ³΄(μ’ν, μΉ΄νκ³ λ¦¬)κ° λͺ¨λΈμ μΈνμΌλ‘ μ¬μ©λ©λλ€. bbox annotationμ COCO formatμΌλ‘ μ κ³΅λ©λλ€. (COCO formatμ λν μ€λͺμ νμ΅ λ°μ΄ν° κ°μλ₯Ό μ°Έκ³ ν΄μ£ΌμΈμ.)
- **Output** : λͺ¨λΈμ bbox μ’ν, μΉ΄νκ³ λ¦¬, score κ°μ λ¦¬ν΄ν©λλ€. μ΄λ₯Ό submission μμμ λ§κ² csv νμΌμ λ§λ€μ΄ μ μΆν©λλ€. (submission formatμ λν μ€λͺμ νκ°λ°©λ²μ μ°Έκ³ ν΄μ£ΌμΈμ

### νκ° λ°©λ²

Test setμ mAP50(Mean Average Precision)λ‘ νκ°
- Object Detectionμμ μ¬μ©νλ λνμ μΈ μ±λ₯ μΈ‘μ  λ°©λ²
- Ground Truth λ°μ€μ Prediction λ°μ€κ° IoU(Intersection Over Union, Detectorμ μ νλλ₯Ό νκ°νλ μ§ν)κ° 50μ΄ λλ μμΈ‘μ λν΄ TrueλΌκ³  νλ¨ν©λλ€.
- Example of IoU  
        ![](https://i.imgur.com/lb9BsAG.jpg)

- metric  
        ![](https://i.imgur.com/7WwZGOb.png)

        
- Example of mAP50  
        ![](https://i.imgur.com/387jIEL.png)

        
    - **Orange**
        - TP = 1, FP = 1
        - μ΄ 2κ°μ Orange λ°μ€ μ€ νλ¨μ λ°μ€ 1κ°λ κ°μ²΄λ₯Ό μ detectionνμμ΅λλ€. (TP) 
            μλ¨μ λ°μ€ 1κ°λ Blue categoryμ ν΄λΉνλ κ°μ²΄λ₯Ό Orange categoryλ‘ μμΈ‘νμκΈ° λλ¬Έμ μλͺ»λ detectionμλλ€. (FP)
            
        ![](https://i.imgur.com/Wk7hrji.png)

        
    - **Blue**
        - TP = 2, FP = 1  
        - μ΄ 3κ°μ Blue λ°μ€ μ€ λ κ°μ λ°μ€λ κ°μ²΄λ₯Ό μ detectionνμμ΅λλ€. (TP) 
            μ°μΈ‘ νλ¨μ λ°μ€λ κ°μ²΄ μμΉλ₯Ό μ νν detectionνμ§ λͺ»νμ΅λλ€. (FP)
        
        ![](https://i.imgur.com/H2ycuEq.png)
        
        - **mAP**
            
            λͺ¨λ  μ΄λ―Έμ§μ κ° ν΄λμ€λ³ AP κ³μ° ν, νκ· λ΄μ΄ μ΅μ’ μ μκ° κ΅¬ν΄μ§λλ€.
            



# λ¬Έμ  μ μ

- __μκ°ν__  

<p align="center"><img src=https://i.imgur.com/UykX7pM.png></p>

μ μ΄λ―Έμ§μμ λ³΄μ΄λ λ°μ κ°μ΄ Classλ³ bbox μμ λΆκ· νμ΄ μ¬νκ³ , λ°°ν°λ¦¬μ κ²½μ° λ°μ΄ν° μκ° 159κ°(νκ·  2,314 κ°)λΏμλλ€.

<p align="center"><img src="https://i.imgur.com/DFKDvXF.png"></p>
<p align="center"><img src="https://i.imgur.com/H27mkEx.png"></p>


β  Class Dependency
- μ λ¨μ§μ κ²½μ° μΌλ° μ°λ κΈ°μ μ’μ΄ λ κ°μ§λ‘ annotationλμ΄ μμ
- μ λ¦¬μ ν¬λͺ νλΌμ€ν±μ΄ λ§€λν νλ©΄, ν¬λͺν¨ λ± μ΄λ―Έμ§μμμ μ μ¬ν νΉμ§μ λ³΄μ
- μμ λ¬Όμ²΄(λΈλμ΄λ μ€ λ±)μ λν background Errorκ° μμ£Ό λμ κ²½ν₯μ λ³΄μ

β‘ Class Imbalance
- Figure 1μμ μ²λΌ Classλ³ bbox μμ λΆκ· νμ΄ μ¬ν¨
- λ°°ν°λ¦¬μ κ²½μ°, λ°μ΄ν° μκ° 159κ°(νκ·  2,314 κ°)λΏ

β’ Various Dataset Environment
- Figure 2 μ κ°μ΄ λ€μν νκ²½μμ μ΄¬μλ μ΄λ―Έμ§





# λ¬Έμ μ λν μ€ν

## μ€ν κ²°κ³Ό

### Issue λ° μ±λ₯ κ°μ μ μν μλ

β  Data Cleansing : Figure 3κ³Ό κ°μ train imageμ μλͺ»λ labelingμ΄λ annotationμ μμ ν΄ μ±λ₯ ν₯μμ μν¨  
β‘ Data Augmentation : Class Imbalance λ° Imageμ μ΄¬μ νκ²½ λ³΄μμ μν λ€μν Augmentation κΈ°λ² μλ  
β Randomfog, Blur, RandomBrightness, Cutmix, Mixup, Mosaic, Resize, normalization, MultiScale, RandomFlip  
β’ Model Selection : Inductive biasλ₯Ό μ΅μννκΈ° μν΄ λ€μν backbone modelμ μ¬μ©νμ¬ νμ΅  
β£ Generalization : μ¬λ¬ Augmentationκ³Ό Noiseλ₯Ό λ£μ΄ μλ,  TTAμλ  
β€ Pseudo Labeling: νμ΅ν λͺ¨λΈλ‘ test λ°μ΄ν°λ₯Ό inferenceν ν, κ·Έ κ²°κ³Όλ‘ μΆκ° νμ΅  
β₯ Ensemble : 1-stage model κ³Ό 2-stage modelμ Ensemble ν¨μΌλ‘μ Robustν λͺ¨λΈ κ°μ  μλ  
β¦ Binary Classification : κ°κ°μ single classλ₯Ό binary classification λ‘ νμ΅  


## μ€ν νμ€ν λ¦¬
<p align="center"><b>Wandbλ₯Ό νμ©ν μ€ν κ΄λ¦¬</b></p>

![](https://i.imgur.com/D44tEOj.png)

<p align="center">Yolo-V5 augmentation test</p>

![](https://i.imgur.com/o9KD9yU.png)

<p align="center">UniverseNet101 augmentation test</p>

![](https://i.imgur.com/h5pEg83.png)


## κ²μ¦ μ λ΅
- classλ³λ‘ APλ₯Ό νμΈνλ©΄μ μ΄λ€ μ νμ νλ¦¬κ³  μλμ§ νμ
- Stratified validationκ³Ό Confusion Matrixλ₯Ό ν΅ν΄ λΆλ₯ λͺ¨λΈ νκ°


<p align="center"><img src="https://i.imgur.com/xK3RTJ3.png"></p>


<br>
<br>

<div>
<center><img src=https://user-images.githubusercontent.com/49435163/146514228-8569412f-46fd-4cc2-8d25-3b0229abba8d.png></center>


</div>





# Modeling λ° Ensemble

<table class="c76"><tbody><tr class="c54"><td class="c63" colspan="1" rowspan="1"><p class="c2"><span class="c0"><b>Model</b></span></p></td><td class="c82" colspan="1" rowspan="1"><p class="c2"><span class="c0"><b>κ°μ  μλ</b></span></p></td><td class="c64" colspan="1" rowspan="1"><p class="c2"><span class="c0"><b>mAP</b></span></p></td></tr><tr class="c5"><td class="c17" colspan="1" rowspan="8"><p class="c2"><span class="c3">UniverseNet101</span></p></td><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Mixup</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.573</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Mosaic / Adam / batch_size 16 / LR 0.0001 / Cutmix Dataset</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.419</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Mosaic / Adam / batch_size 16 / LR 0.0001</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.451</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">HueStauration / Adam / batch_size 16 / LR 0.0001</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.619</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">&nbsp;RandomFog / batch_size 16 / LR 0.0001</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.623</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">RandomBrightness / batch_size 16 / LR 0.002</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c0"><b>0.624</b></span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Blur, RandomFog, RandomBrightness, Mixup / Adam / batch_size 16 / LR 0.0001 /Data Cleaning</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.613</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Data cleaning / RandomBrightness / batch_size 16 / LR 0.002</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.590</span></p></td></tr><tr class="c5"><td class="c17" colspan="1" rowspan="5"><p class="c2"><span class="c3">Swin-T,S</span></p></td><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Swin-T / Adam / batch_size 4 / LR 0.0001 </span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.523</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Swin-T / MultiScale / Adam / batch_size 4 / LR 0.0001</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.550</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Swin-S / MultiScale / AdamW / batch_size 4 / LR 0.0001</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.561</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Swin-S / MultiScale, Mixup / AdamW / batch_size 4 / LR 0.0001</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.571</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">Swin-S / Randomfog, RandomBrightnessContrast, ShiftScaleRotate, MultiScale, Mixup / AdamW / batch_size 4 / LR 0.0001</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c0"><b>0.586</b></span></p></td></tr><tr class="c5"><td class="c17" colspan="1" rowspan="5"><p class="c1"><span class="c3"></span></p><p class="c2"><span class="c3">Yolo-V5</span></p></td><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">baseline (Yolo v5x6 default) / 300 epoch</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c0"><b>0.586</b></span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">label smoothing (T=0.05) / 300 epoch</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.583</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">single class / 300 epoch </span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.008</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">random fog / 50 epoch</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.573</span></p></td></tr><tr class="c5"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">pseudo labeling (conf_threshold=0.6) / train data(10epoch x 3), pseudo data(10epoch x 2) λ²κ°μκ°λ©° νμ΅ / pseudo data νμ΅μ obj loss μ μΈ / 50 epoch</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.559</span></p></td></tr><tr class="c35"><td class="c17" colspan="1" rowspan="3"><p class="c2"><span class="c13">PVTv2-B3</span></p></td><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c13">baseline epoch 30 / batch size 4 / scheduler step / LR 0.002 / </span><span class="c97">fp16</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.541</span></p></td></tr><tr class="c35"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">batch size 3 / LR 0.0001 / &nbsp;Adam / score_thr = 0</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c0"><b>0.573</b></span></p></td></tr><tr class="c35"><td class="c8" colspan="1" rowspan="1"><p class="c2"><span class="c3">batch size 2 / LR 0.0001/ mixup, RandomFog, blur, randbright / Adam / Data cleaning</span></p></td><td class="c23" colspan="1" rowspan="1"><p class="c2"><span class="c3">0.526</span></p></td></tr></tbody></table>

λ μμΈν κΈ°λ‘μ [λλ³΄κΈ°...](https://docs.google.com/spreadsheets/d/1xw11I8pUZY8CGaE0jXeE4KGokvK-zbpxHdKKYsyt_SI/edit#gid=265349216)

## μ΅μ’ Ensembleλ λͺ¨ν
<p align="center"><img src="https://i.imgur.com/2BvTb4c.png"></p>
κ° modelλ³λ‘ κ°μ₯ LB scoreκ° μ’μλ λ²μ  5κ°λ₯Ό Ensembleνμ¬ μ΅μ’ λͺ¨λΈμ μμ±  

# νκ³ 

## μνλ μ 
- mmdetection λΌμ΄λΈλ¬λ¦¬λ₯Ό νμ©νμ¬ object detectionμ μ λ°μ μΈ taskλ₯Ό μνν΄ λ³Ό μ μμμ΅λλ€.
- mAP, NMS, WBFλ± object detectionκ³Ό κ΄λ ¨λ μ©μ΄λ€μ λν΄ κ³΅λΆ ν  μ μμμ΅λλ€.
- object detectionμ κ΄λ ¨λ λ€λ₯Έ λνλ€(Kaggle, Dacon)μ μ°Ύμλ³΄κ³  λνμμ νμ©λ κΈ°λ²λ€μ μ΄λ² λνμ μ μ©μμΌ λ΄μΌλ‘μ¨ μ±λ₯ λ³νλ μ€μ λ‘ μ μ©μμΌ°μ λμ μ΄λ €μ λ±μ κ²½νν΄λ³΄κ³  μ΄μ κ΄λ ¨λ λ΄μ©μΌλ‘ νμλ€κ³Ό μν΅νμ¬ μ±μ₯μ λλͺ¨νμ΅λλ€.
- mmdetection μΈμ yolov5, Universenetκ³Ό κ°μ λ€λ₯Έ λΌμ΄λΈλ¬λ¦¬λ₯Ό μ¬μ©ν΄ λ³΄λ λ±  λ€μν μλλ₯Ό νμμ΅λλ€.

![](https://i.imgur.com/LVSLYC5.png)


## μμ¬μ λ μ 

- mmdetectionκ³Ό κ΄λ ¨λ λ€μν λΌμ΄λΈλ¬λ¦¬λ₯Ό μ²μ νμ©ν¨μ μ΄λ €μμ΄ μμ΄μ λ΄κ° μνλ λͺ¨λΈμ κ΅¬ννλλ° μκ°μ΄ μ€λ κ±Έλ Έμ΅λλ€. μλ‘­κ² λ°°μκ°λ€λ λλλ³΄λ€ mmdetection λΌμ΄λΈλ¬λ¦¬λ₯Ό ν΅ν΄ κΈ°κ³μ μΌλ‘ νλΌλ―Έν° νλμ νμ¬ μ±λ₯μ ν₯μμν¨λ€λ λλμ΄ κ°ν΄μ μμ¬μ μ΅λλ€.
- object detectionμ μ²μ μλ¬Έν¨μ μμ΄μ λ€μν νμ€νΈλ₯Ό ν΄λ΄μΌ νλλ° κ²°κ³Όλ₯Ό λ³΄κΈ°κΉμ§μ μκ°μ΄ λλ¬΄ μ€λ κ±Έλ Έκ³ , μ΄λ‘ μΈν΄ λ€μν μ€νμ κΈ°κ° λ΄μ ν΄κ²°νμ§ λͺ»νμ΅λλ€.
- test datasetκ³Ό μ μ¬ν validation datasetμ μ°ΎκΈ° μ΄λ €μ μ°κ΅¬κ° μ§νλ μλ‘ modelμ κ°μ μν€κΈ° μν λλ ·ν νλ¨μ κ·Όκ±°κ° λΆμ‘±νμ΅λλ€.
- LB mAPλ₯Ό λμ΄κΈ° μν΄μλ bounding boxλ₯Ό λ§μ΄ μΉλ κ²μ΄ ν¨κ³Όκ° μμκ³  κ·Έλ¬λ€ λ³΄λ λμΆλ κ²°κ³Όλ₯Ό νμΈνμλ μ΄κ±Έ detectionνλ€κ³  ν  μ μλμ§ μλ¬Έμ΄ λ€μκ³  mAPκ° νκ° μ§νλ‘ μ ν©νκ° μλ¬Έμ΄ λ€μμ΅λλ€.


<table align="center">
    <tr>
        <td><img width="340" src="https://i.imgur.com/IjbLt9r.jpg" /><br/>
            <p align='center'> mAP 0.672</p>
        </td>
        <td><img width="300" src="https://i.imgur.com/OuI6iNY.png" /><br/>
            <p align='center'> mAP 0.482</p>
        </td>
    </tr>
</table>

## νμλ€μ νλ§λ

- νκ±΄μ° : μΈλΆ λΌμ΄λΈλ¬λ¦¬λ₯Ό μ¬μ©ν  λλ ν­μ κ²μ¦νκ³  μ¬μ©ν΄μΌνλ€λ μ μ λ€μ νλ² λλΌκ² λμμ΅λλ€.
- λ°μ€ν : μ²« object detection λνλ₯Ό κ²½νν¨μΌλ‘μ λ§μ μ΄λ €μμ΄ μμμΌλ νμλ€κ³Όμ μν΅μΌλ‘ μ ν΄κ²°ν΄λκ°κ³ , μμΌλ‘λ μ΄λ° object detection taskμ λν κ°μ μ»μ μ μμ΄μ μ’μμ΅λλ€. νμ λͺ¨λ λνλ₯Ό μ΄μ¬ν μ§νν΄μ£Όκ³  κ°μ΄ κ³ λ―Όν΄μ£Όμ΄μ κ°λμ΄μμ΄μ~!
- νμν : λΌμ΄λΈλ¬λ¦¬μ μ΅μν΄μ§λλ° μκ°μ΄ μ€λ κ±Έλ € λ λ§μ μ€νμ λͺ»νλλ° λ€μ λνμλ λ λ§μ μλλ₯Ό ν΄λ³΄κ³  μΆμ΅λλ€!
- ν©μμ : μ΄μ  κ°μ μ‘μκ°λ κ² κ°μ΅λλ€. λ€μ λν λλ λ μκ°λ΄μλ€.
- λ°λ²μ : λλ²μ§Έ competitionμ΄μ§λ§ μμ§λ λΆμ‘±νκ² λ§λ€κ³  λλΌλ λνμμ΅λλ€. μμΌλ‘λ μ‘°κΈ λ μ²΄κ³μ μΌλ‘ λνλ₯Ό μ§νν΄μΌκ² λ€λ κ±Έ κΉ¨λ¬μμ΅λλ€.
- μν¬μ : νμμ μ€μνλ€κ³  μκ°ν΄ μλλ° λ€μν λΌμ΄λΈλ¬λ¦¬λ‘ μ€νμ μ§νν΄μΌ νλ μν©μμλ μ°μ μ νμ§ μμ νμλ μλ€κ³  κΉ¨λ«κ² λμκ³ , μ λ°μ μΈ detection taskλ₯Ό μμκ° μ μμλ€λ μ μμ μλ―Έ μμ§λ§ λΌμ΄λΈλ¬λ¦¬ νλλ§ νλ€ λλ¬λ€κ³  μκ°μ΄ λ€κΈ°λ ν΄μ μμ¬μ΄ λ§μμ΄ λ¨μ΅λλ€. λͺ¨λ μκ³  λ§μΌμ¨μ΄μ!
- μ‘°νμ : Object detection λͺ¨λΈλ€μ μ§μ  νμ΅ν΄λ³Ό μ μμ΄μ μ’μμΌλ, λͺ¨λΈ κ΅¬μ‘°μ λν΄ κΉμ΄μκ² νμνμ§ λͺ»ν λ±μ μμ¬μλ λ§μ΄ λ¨λ λνμμ΅λλ€. νμλΆλ€ λͺ¨λ μκ³ λ§μΌμ¨μ΄μ!

# Reference

<p><span style="background-color:#EEEEEE;">λ€μ΄λ² μ»€λ₯νΈμ¬λ¨ - μ¬νμ© μ°λ κΈ° λ°μ΄ν°μ / CC BY 2.0<br/>
https://stages.ai/competitions/76/overview/description
</span></p>

