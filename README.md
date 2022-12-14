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
