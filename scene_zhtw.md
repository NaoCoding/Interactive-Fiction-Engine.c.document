## scene / subscene / 場景與對話

這個文檔會引導您建立場景或對話

## 場景

#### 開始遊戲的第一個場景

設定場景 start 為 第一個場景

```
first_scene:[場景名稱]
ex. first_scene:start
```

#### 新的場景

宣告場景後，接下來的程式（直到下一個場景或對話）<br>
皆會被視為該場景的內容

```
scene.[場景名稱]
ex. scene.start
```

#### 角色移動來切換場景

宣告角色移動到地圖左右邊緣會切換到指定場景

```
change_scene.character.[right / left].[場景名稱]
ex. change_scene.character.left.hallway
```

## 對話

#### 新的對話

宣告對話後，接下來的程式（直到下一個場景或對話）<br>
皆會被視為該對話的內容

```
subscene.[場景名稱]
ex. subscene.start
```


#### 結束對話

事實上，結束對話也可以被視為一個＂對話＂
宣告對話後，接下來的程式（直到下一個場景或對話）<br>
皆會被視為該對話的內容

```
close_subscene.[場景名稱]
ex. close_subscene.ending
```
