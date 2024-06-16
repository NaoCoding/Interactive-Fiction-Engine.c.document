## NPC / 角色

這份文件會引導您去建立不同的角色

## 開始創建角色

#### 設定角色數量

這是最重要的，必須先有這個後才能開始建立不同角色。<br>
這會影響到 engine 去 calloc structure的大小。
* 超出數量會導致引擎出現 Segmentation Fault
* 請確認自己開的數量

```
character.count:[int]
ex. character.count:10
```

#### 創建一個新角色

命名請勿重複，否則會有其中之一不會被使用 <br>
以下範例為創建一個角色名為 Andy Lu
```
character.create:[string]
ex. character.create:Andy Lu
```

## 設定角色照片（無動畫）

#### 建立一個新照片

引擎支援同一隻角色有很多照片 <br>
因此，設定照片的同時需要設定照片的名稱

```
character.[角色名稱].src:[圖片名稱],[路徑]
ex. character.Ichiha.src:normal_stand,"images/character01/character01.png"
```

#### 顯示與隱藏圖片

* 若圖片名稱不存在會導致 Segmentation Fault
* 請確認自己設定的圖片名稱

```
character.[角色名稱].[hide / show]:[圖片名稱]
ex . character.Ichiha.hide:normal_stand2
ex . character.Andy Lu.show:standing_pose
```

#### 設定照片的 css style

與對話框同樣支援 place 和 style
詳情見對話框的文檔

* 若圖片名稱不存在會導致 Segmentation Fault
* 請確認自己設定的圖片名稱

```
character.Ichiha.place:normal_stand4,"auto","80%","10%","0%"
character.Andy Lu.style:zIndex,3
```

## 設定控制角色（角色移動）

#### 開始控制角色

```
character.[角色名稱].control.start
ex. character.Ichiha.control.start
```

#### 結束控制角色

```
character.[角色名稱].control.stop
ex. character.Ichiha.control.stop
```

## 角色動畫

#### 設定動畫角色的顯示與隱藏

```
character.[角色名稱].[moving_hide / moving_show]
ex . character.Ichiha.moving_show
```

#### 設定動畫角色的 css style

與對話框同樣支援 place 和 style
詳情見對話框的文檔

* 若圖片名稱不存在會導致 Segmentation Fault
* 請確認自己設定的圖片名稱

```
character.Ichiha.moving_place:normal_stand4,"auto","80%","10%","0%"
character.Andy Lu.moving_style:zIndex,3
```

#### 建立動畫圖片來源

建立一個角色動畫的index
```
character.[角色名稱].moving.1:[圖片路徑]
character.Anett.moving.1:"images/classroom/Anett1.png"
```

#### NPC 站立時的動畫

為NPC，非控制時的角色

```
character.[角色名稱].moveAnimation:[開始的index, 結束的index]
ex. character.Anett.moveAnimation:1,18
```

#### idle（不移動時的動畫）

須為控制的角色

```
character.[角色名稱].control.standingAnimation:[開始的index, 結束的index]
ex. character.Ichiha.control.standingAnimation:11,18
```

#### 移動時的動畫

角色會在移動時循環從開始到結束的動畫

```
character.[角色名稱].control.movingAnimation:[開始的index, 結束的index]
ex. character.Ichiha.control.movingAnimation:11,18
```

## 點擊角色後進入 / 退出對話

與對話框使用方式一樣
詳情見對話框的文檔

```
ex. character.Anett.subscene_open.subsceneexample01
```
