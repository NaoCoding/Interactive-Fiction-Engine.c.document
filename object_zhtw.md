## object / 場景道具

任何場景內可以點擊的特定道具 <br>

#### 建立新的道具

```
object.create.[道具名稱]
ex. object.create.door
```

#### 道具的 css style 設定

語法與dialogBox完全相同
詳情見對話框的文檔

```
object.src.[道具名稱].place
object.src.[道具名稱].style
```

#### 顯示與隱藏道具

語法與dialogBox完全相同
詳情見對話框的文檔

```
object.src.[道具名稱].show
object.src.[道具名稱].hide
```

#### 道具的圖片來源

```
object.src.[道具名稱].[圖片路徑]
```

#### 道具點擊後切換場景 / 對話

語法與dialogBox完全相同
詳情見對話框的文檔

```
object.click.[道具名稱].scene_open.[場景名稱]
object.click.[道具名稱].subscene_open.subscene + [對話名稱]
```
