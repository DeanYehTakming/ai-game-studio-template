# AI 造物工坊

用 GitHub Codespaces 和 Copilot Chat，在瀏覽器裡做出自己的網頁小遊戲。不需要在電腦上安裝任何軟體。

## 開始之前

使用 GitHub 的 **Use this template → Create a new repository** 建立自己的儲存庫，再選擇 **Code → Codespaces → Create codespace on main**。

## 操作步驟

1. 在檔案總管中對 `index.html` 按右鍵，選擇 **Show Preview**，就能看到遊戲畫面。
2. 複製 `spec.template.md` 並命名為 `spec.md`，填寫遊戲規格後，請 Copilot Chat 根據規格改寫 `index.html`。
3. 要儲存進度時，打開左側的 **Source Control**，輸入提交訊息，按 **Commit**；如果要同步到 GitHub，再按 **Sync Changes** 或 **Push**。
4. 下課時，到 [GitHub Codespaces](https://github.com/codespaces) 找到你的 Codespace，點選旁邊的 **⋯ → Stop codespace**，避免繼續使用運算時間。

## 檔案說明

| 檔案 | 用途 |
| --- | --- |
| `index.html` | 你的遊戲。所有 HTML、CSS、JavaScript 都寫在這一個檔案裡。 |
| `spec.template.md` | 規格書範本。複製成 `spec.md` 後填寫。 |
| `.github/copilot-instructions.md` | 給 Copilot 的專案規則，Copilot Chat 會自動讀取。 |
| `.devcontainer/devcontainer.json` | Codespace 的環境設定，一般不需要修改。 |

## Copilot Chat 提示詞範例

可以直接複製貼到 Copilot Chat，再依自己的情況修改。

- 做出第一版：`請依照 spec.md 改寫 index.html，做出可以玩的第一版。`
- 規格不確定時：`請先讀 spec.md，列出規格中不清楚的地方並問我，先不要寫程式。`
- 一次只改一件事：`請只修改主角的移動速度，讓它快一點，其他地方不要動。`
- 修 Bug：`我按空白鍵時主角不會跳。請找出原因，只改必要的地方，並說明為什麼。`
- 看不懂程式：`請用簡單的話解釋 index.html 裡的遊戲迴圈在做什麼。`

小技巧：一次只請 Copilot 做一件事，每完成一個能正常運作的功能就 Commit 一次，改壞了才救得回來。

## 常見問題

- **預覽畫面沒有更新**：先確認檔案已經儲存（本專案預設會自動儲存），再按預覽視窗上方的重新整理按鈕。
- **右鍵選單沒有 Show Preview**：Codespace 剛開啟時擴充功能還在安裝，等一兩分鐘後再試；還是沒有就重新整理瀏覽器頁面。
- **遊戲畫面一片空白或按鍵沒反應**：在預覽視窗按右上角的 **⋯ → Open Devtools Pane** 查看錯誤訊息，把紅色的錯誤訊息貼給 Copilot Chat 請它修正。
- **Copilot 改完之後遊戲壞掉了**：在 **Source Control** 對 `index.html` 選擇 **Discard Changes**，就能回到上一次 Commit 的版本。
- **Copilot 做出來的和規格不一樣**：回頭檢查 `spec.md` 是不是寫得不夠具體，補上細節後再請 Copilot 修改。

課程手冊連結：請講師在發布前補上。
