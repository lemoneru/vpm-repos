# LEMONERU VPM Packages

LEMONERU 製 VRChat 向けツールの VPM リポジトリです。
VCC (VRChat Creator Companion) / ALCOM に登録すると、各プロジェクトへ数クリックで導入・更新できます。

## 登録方法

**ワンクリック登録（VCC / ALCOM 共通）**

👉 <https://lemoneru.github.io/vpm-repos/> を開いて「VCC に追加」ボタンを押してください。

**手動で登録する場合**

1. VCC / ALCOM の設定画面で「Packages」→「Add Repository」を開く
2. 次の URL を貼り付けて追加する

```
https://lemoneru.github.io/vpm-repos/index.json
```

## ベータ版の表示について

`3.0.0-beta.2` のようなプレリリース版は、VCC の
**Settings → Packages → Show Pre-release Packages** を ON にすると一覧に表示されます。
（ALCOM は設定不要で表示されます）

## トライアル版とコンプリート版

VCC / ALCOM から入れた直後の Avatar Blink Fix は**トライアル版**として動作します（まばたき用 BlendShape 1 つの修正・プレビュー・復元）。
BOOTH（<https://lemoneru.booth.pm/items/7074770>）で購入すると**解除キー**（`AvatarBlinkFix_UnlockKey.unitypackage`）が付いています。プロジェクトに 1 回インポートすると、同じ PC の全プロジェクトで**コンプリート版**になります。
保存されるのは Unity の EditorPrefs `AvatarBlinkFix_UnlockSecret` の 1 項目だけで、外部通信はありません。取り消しは Tools → Avatar Blink Fix の［トライアル版に戻す］から。

**Trial / Complete (EN)**: Right after installing via VCC / ALCOM, Avatar Blink Fix runs as the **trial edition** (fixes one blink BlendShape). Buyers on BOOTH get an **unlock key** (`AvatarBlinkFix_UnlockKey.unitypackage`); import it once → **complete edition** on this PC. Only one EditorPrefs value (`AvatarBlinkFix_UnlockSecret`) is stored, no network access. Revoke anytime via Tools → Avatar Blink Fix → [Return to trial].

## 2.x や unitypackage 版が入っているプロジェクトへ入れるとき

3.0 は `Packages/com.lemoneru.avatar-blink-fix/` に入ります。以前の版が `Assets/LEMONERU/Avatar Blink Fix/` に残っていると二重になり正しく動きません。
**追加する前に、そのフォルダの中の `Editor` と `Runtime`（あればプレハブ 2 つ・README・CHANGELOG・package.json も）を削除**してください。`Data`・`Animation`・`json` は残して構いません（修正の記録・生成したアニメーション・追加したプリセット。3.0 もそのまま使います）。
先に 3.0 を入れてしまってもエラーが出ていなければ、Tools → Avatar Blink Fix を開くと「古い Avatar Blink Fix のファイルが残っています」と案内が出て、［旧本体を削除］でツール本体のファイルだけをごみ箱へ移動できます。

**Upgrading from 2.x (EN)**: 3.0 lives in `Packages/`. Before adding it, delete `Editor` and `Runtime` inside `Assets/LEMONERU/Avatar Blink Fix/` (keep `Data`, `Animation`, `json`). If already added and the window still opens, use **[Delete old files]** shown at the top of Tools → Avatar Blink Fix.

## 収録パッケージ

| パッケージ | 説明 |
|---|---|
| Avatar Blink Fix | 改変で壊れたまばたきを数クリックで修正する VRChat アバター向けツール |

## サポート

- BOOTH: <https://lemoneru.booth.pm/>
