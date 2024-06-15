## status / 狀態欄與背包

狀態欄和背包皆可隨時更改 <br>
豐富遊戲程度與使遊戲增加一些判斷或過關條件

#### 角色圖片

```
status.photo.[圖片路徑]
```

#### 角色名稱

```
status.name.[名稱]
```

## 狀態

#### 新增狀態

最多可以有八種狀態

```
status.value.new.[狀態名稱]
ex. status.value.new."飽食度"
```

#### 狀態數字改動

數字會增加（負數則減少）
重複的來源不會重複增加

```
status.value.add.[狀態名稱].[來源名稱].[增加的值]
ex. status.value.add."飽食度"."碰到餐廳".10
```

## 物品

#### 新增物品

最多可以有九種物品

```
status.inventory.new.[物品名稱]
ex. status.inventory.new."書本"
```
#### 物品圖片
```
status.inventory.src.[圖片路徑]
ex. status.inventory.src."images/example.png"
```
#### 獲得物品
```
status.inventory.new.[物品名稱]
ex. status.inventory.get.書本
```



## 選項出現的條件

#### 需擁有道具

設定需擁有甚麼道具才會開啟選項幾

```
status.require.inventory.[道具名稱].[選項幾]
```

#### 某狀態達到多少分

設定目標狀態達到多少分才會開啟選項幾

```
status.require.value.[狀態名稱].[多少分].[選項幾]
```

