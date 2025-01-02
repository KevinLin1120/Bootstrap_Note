# Layout Grid

## What

1. Bootstrap 使用 12 格的格線系統

## Concept

1. 使用 `container` 跟 `row` 來做網格 (透過網格的大小控制內容大小；可將內容寬度設為 100%)

2. 再自訂容器來裝內容

3. 分為 **自動欄寬**, **固定欄寬** 兩種寫法

4. 透過 col-XX-y 來做成 RWD

5. bootstrap grid 使用 flexbox 製成

## How to start

1. 使用 `.container` 來做一個定寬容器 (若想坐滿版的 `.container-fluid`)

2. 在內部使用 `.row`

3. row 內放 `.col-x-y` (x 為不同容器寬度設定, y 為有幾欄)

4. 在 row 使用 `g-X` (X 為大小)，可控制 col 間距

5. 對 col 使用 `order-XX-Y` (XX: 裝置，Y: 大小)，可控制元素順序 (甚至依照不同裝置而更動)

## QA

1. Q: 怎麼做 5 欄

   A: 直接寫 `.col`， 不用給大小 Ex. `<div class=".col">` (自動欄寬)

2. Q: 自動欄寬時，怎麼控制不同螢幕時有幾欄

    A: 在 `.row` 中加入 `.row-cols-XX-N` (XX: 裝置螢幕寬, N: 此寬度時有幾**欄**)

3. Q: 如果想放 3 個 col，但每個 col 只想有 col-3 的寬度，又要讓內容置中，要怎麼做

    A: 在 `.row` 中加入 `.justify-contnet-center`

## Description

1. Breakpoint 斷點: 根據不同螢幕寬度來給定不同斷點，Ex. >=576px -> `sm`

2. `container`: 定寬容器，控制寬度

3. `row`:

    1. display: flex: 讓內容橫向排列

    2. flex-wrap: 讓內容可以換行

    3. margin-x

4. `justify-content-{center | start | end | between | around}`: 使用 css 中的

    - `justify-content: center`

    - `justify-content: {flex-start | flex-end}`: css 的 flex

    - `justify-content: {space-between | space-around}`
