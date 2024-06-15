## dialogBox / 對話框

這份文件會引導您在您的劇本檔中開始撰寫對話框 <br>

## 基礎

#### 顯示對話框

```
dialogBox.show
```

#### 隱藏對話框

```
dialogBox.hide
```

#### 對話框的大小調整

此為支援 css style 去調整對話框的屬性

```
dialogBox.place: width, height, left, top 
ex . dialogBox.place:"100%","100%","0px","0px"
```

#### 對話框的css style調整

此為支援 css style 去調整對話框背景圖片的屬性

```
dialogBox.style: target , value
ex . dialogBox.style:zIndex, 1
```

## 對話框背景

#### 對話框的背景圖片

```
dialogBox.background.src: [路徑]
ex. dialogBox.background.src:"images/dialogBox.png"
```

#### 對話框背景圖片的大小調整

此為支援 css style 去調整對話框背景圖片的屬性

```
dialogBox.background.place: width, height, left, top 
ex . dialogBox.background.place:"100%","100%","0px","0px"
```

#### 對話框背景圖片的css style調整

此為支援 css style 去調整對話框背景圖片的屬性

```
dialogBox.background.style: target , value
ex . dialogBox.background.style:zIndex, 1
```

## 對話框內容

#### 設定對話框內容

以下範例為將內容設定為 Hello World

```
dialogBox.content.set: [string]
ex . dialogBox.content.set:"Andy Lu"
```

#### 對話框內容的大小調整

此為支援 css style 去調整對話框內容的屬性

```
dialogBox.content.place: width, height, left, top 
ex . dialogBox.content.place:"100%","100%","0px","0px"
```

#### 對話框內容的css style調整

此為支援 css style 去調整對話框內容的屬性

```
dialogBox.content.style: target , value
ex . dialogBox.content.style:zIndex, 1
```

## 對話框正在說話者

#### 設定對話框正在說話的人

以下範例為將正在說話的人設定為 Andy Lu

```
dialogBox.speaker.set: [string]
ex . dialogBox.speaker.set:"Andy Lu"
```

#### 對話框正在說話者的大小調整

此為支援 css style 去調整對話框正在說話者的屬性

```
dialogBox.speaker.place: width, height, left, top 
ex . dialogBox.speaker.place:"100%","100%","0px","0px"
```

#### 對話框背正在說話者的css style調整

此為支援 css style 去調整對話框正在說話者的屬性

```
dialogBox.speaker.style: target , value
ex . dialogBox.speaker.style:zIndex, 1
```

## 對話框點擊

#### 切換到下一個對話

以下範例為設定點擊對話框後切換到 test 的對話

```
dialogBox.click.subscene_open:subscene + [subscene_name]

ex. dialogBox.click.subscene_open:subscenetest
```

#### 關閉對話

以下範例為設定點擊對話框後關閉 test 的對話

```
dialogBox.click.subscene_close:subscene + [subscene_name]

ex. dialogBox.click.subscene_close:subscenetest
```

#### 切換場景

以下範例為設定點擊對話框後切換到 classroom 的場景

```
dialogBox.click.scene_open:[scene_name]

ex. dialogBox.click.scene_open:classroom
```
