## option / 選擇與選項


## 顯示/隱藏 及 css style

#### 顯示選項

```
option.show.[選項幾]
ex. option.show.1
```

#### 隱藏選項

```
option.hide.[選項幾]
ex. option.hide.1
```

#### 選項的大小調整

此為支援 css style 去調整對話框的屬性

```
option.place.[選項幾]: width, height, left, top 
ex . option.place.1:"100%","100%","0px","0px"
```

#### 選項的css style調整

此為支援 css style 去調整對話框背景圖片的屬性

```
option.style.[選項幾]: target , value
ex . option.style.1:zIndex, 1
```

## 選項的圖片或內容

#### 選項圖片

```
option.src.[選項幾].[圖片路徑]
```

#### 選項內容文字
```
option.content.[選項幾].[內容文字]
```

## 選項切換場景 / 對話

#### 切換場景
```
option.set.scene_open.[場景名稱]
```

#### 切換對話
```
option.set.subscene_open.subscene+[對話名稱]
```

#### 關閉對話
```
option.set.subscene_close.subscene+[對話名稱]
```
