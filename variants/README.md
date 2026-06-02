# 投遞版履歷（variants）

每份要投的 JD 建議複製一份主檔再改，避免改亂 `base.md`。

## 建立新投遞版

```bash
cp ../base.md ./公司名-職稱.md
```

## 常改項目（對齊 `@resume-target-jd` 的 🔴 建議）

1. **Summary** — 第一句對齊 JD 的 product area
2. **經歷順序** — 最相關的 `###` 區塊上移
3. **子彈句** — 在對應 `####` 下改寫或補指標
4. **Skills** — 註解掉與該 JD 無關的類別（勿刪 `base.md`）
5. **刪減** — 整段 KaChick / 工設經歷可縮短或移到文末

## 與 HTML 同步

| Markdown | HTML（列印 PDF） |
|----------|------------------|
| `resume/base-0522.md` | `resume/resume.html`（通用版） |
| `resume/variants/LineBank.md` | `resume/resume-LineBank.html` |

改完 variant 後同步對應 HTML，瀏覽器開啟後列印 PDF。通用版改 `base-0522.md` 時同步 `resume.html`。

對話中審閱請 `@variants/xxx.md` + `@targets/xxx/jd.md`（或 `@.cursor/active-target.md`），**不必重貼** JD／履歷全文。slug 需與 `targets/` 資料夾同名。
