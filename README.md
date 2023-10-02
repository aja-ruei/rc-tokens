## 2023-10-02 更新項目
- 新增 $sys-color-bg-chosen

## 2023-07-21 更新項目
- 調整 themes 數值
  - $sys-color-bg-decorative-secondary
  - $sys-color-text-highlight
  - $sys-color-border-highlight
  - $sys-color-icon-dark
  - $sys-color-icon-inverse
  - $sys-color-infographics-highlight
- 新增 themes
  - $sys-color-icon-success
- 調整 variables 數值
  - $color-decorative-neon-blue-200: #27dbe7;

## 2023-07-05 更新項目
- 新增 $sys-color-bg-decrease、$sys-color-bg-increase、$sys-color-text-default、$box-shadow-bottom-nav
- 調整 themes/_dark $sys-color-text-tertiary
- 調整 themes/_light $sys-color-bg-secondary
- 調整 abstracts/_variables：$color-functional-red-200、$color-functional-green-200 數值

## 2023-06-06 更新項目
- 新增 $sys-color-bg-light、$sys-color-bg-contrast、$sys-color-icon-inverse、$sys-color-border-inverse、$sys-color-text-inverse、$box-shadow-bottom-nav
- 調整 $color-functional-red-100 數值

## 2023-04-25 更新項目
- 新增 $sys-color-legacy-base 用於舊頁面特殊背景色
- 調整 $color-brand-secondary-400、$color-functional-green-100 與 $color-functional-orange-100 數值

## 2023-04-10 更新項目
- 新增 $sys-color-border-pressed、$sys-color-icon-onBrand
- 更新 light mode 中 $sys-color-border-highlight


## 2022-12-28 更新項目

### 新增適用於舊頁面的 tokens
- 第一階段目標為更新舊頁面以符合新版色彩風格，目前舊頁面的元件未必適配於新版元件樣式，所以新增一組 `$sys-color-legacy` 用於快速置換舊頁面中帶有狀態的元件的 background-color、border-color 等，及舊頁面中的特殊標籤、強調樣式的底色，與帶有功能的文字，如文字按鈕。舊頁面的置換邏輯請參閱文件，請留意新版的頁面中不要使用這個分類的變數。
  

## 2022-12-14 更新項目

### 1. 調整分類
- 將原先的 `$sys-color-container` 分類整併至 `$sys-color-bg-`，背景色收斂為 `surface` 與 `bg` 兩種：

  - `$sys-color-surface-` 用於帶有陰影的元件背景，亦即帶有 `box-shadow` 值
    - `$sys-color-surface-inverse1` 可能搭配 `$box-shadow-bottom-sheet`、`$box-shadow-nav` 或 `$box-shadow-drag` 依元件選擇適配的陰影樣式
    - `$sys-color-surface-inverse2` 則可能搭配 `$box-shadow-card` 或 `$box-shadow-popup`
  
  - 帶有陰影的物件上方不會再放置帶有陰影的元件
  
- `$sys-color-bg-`則用於沒有陰影的元件背景
- 背景色中帶有 `-inverse-` 者，用於頁面（背景遮罩）上的第一層元件或牌卡

### 2. 移除未使用 token
- $sys-color-surface-secondary
- $sys-color-icon-decorative-primary
- $sys-color-icon-decorative-secondary
- $box-shadow-base

### 3. 命名更新對照
- $sys-color-surface-inverse  變更為 $sys-color-surface-inverse1
- $sys-color-surface-primary 變更為 $sys-color-surface-inverse2
- $sys-color-bg-default 變更為 $sys-color-bg-base
- $sys-color-bg-primary 變更為 $sys-color-bg-brand
- $sys-color-bg-nav 變更為 $sys-color-bg-inverse
- $sys-color-container-primary 變更為 $sys-color-bg-primary
- $sys-color-container-secondary 變更為 $sys-color-bg-secondary
- $sys-color-container-tertiary 變更為 $sys-color-bg-tertiary
- $sys-color-icon-tab-default  變更為 $sys-color-icon-nav-default
- $sys-color-icon-tab-selected 變更為 $sys-color-icon-nav-selected
- $sys-color-text-on-primary 變更為 $sys-color-text-on-brand

### 待新增
- layout tokens (padding, margin, grid)
