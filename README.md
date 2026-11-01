# ORIVEIL

Post-match review and team tools for VALORANT players (Windows, free).

VALORANT プレイヤーのための、試合後の振り返りとチームプレイ支援ツール（Windows 用・無料）。

- Website / 公式サイト: https://oriveil.app/
- Privacy Policy / プライバシーポリシー: https://oriveil.app/en/privacy.html
- Terms of Service / 利用規約: https://oriveil.app/en/terms.html
- Reviewer Guide / 審査・API 利用説明: https://oriveil.app/en/guide.html
- Contact / お問い合わせ: https://oriveil.app/en/contact.html

> This repository only hosts release files (installers). The source code is not published here.
>
> このリポジトリは配布ファイルの置き場所です。ソースコードは公開していません。

## Download / ダウンロード

Download from the [Releases](../../releases) page.

| File | Description | Size |
| --- | --- | --- |
| `ORIVEIL-Setup-1.1.1.exe` | Installer (per-user, no admin rights) / インストーラー（管理者権限不要） | 117 MB |
| `ORIVEIL-Portable-1.1.1.exe` | Portable (no installation) / ポータブル版（インストール不要） | 371 MB |
| `ORIVEIL-1.1.1-SHA256SUMS.txt` | SHA-256 checksums / チェックサム | — |

Requirements / 動作環境: Windows 10 / 11 (64-bit)

### Verify the download / ダウンロードしたファイルの確認

```powershell
Get-FileHash .\ORIVEIL-Setup-1.1.1.exe -Algorithm SHA256
Get-FileHash .\ORIVEIL-Portable-1.1.1.exe -Algorithm SHA256
```

Compare the result with `ORIVEIL-1.1.1-SHA256SUMS.txt`.

表示された値がチェックサムファイルと一致することを確認してください。

The files are not code-signed yet, so Windows SmartScreen may show a warning on first launch.

現在の配布ファイルにはコード署名がないため、初回起動時にSmartScreenの警告が出ることがあります。発行元とチェックサムを確認し、安全性に納得できる場合のみ実行してください。

## Status / 提供状況

Riot Games Production API application is being prepared. Riot account linking and official match data are not currently available. Until approval and integration, ORIVEIL runs in Demo Mode with sample data labeled "DEMO".

Riot Games Production APIは現在申請準備中です。公式アカウント連携と試合データ取得はまだ利用できません。承認と連携実装が完了するまでは、デモモードで動作します。

## Upgrading from VALO NEXUS / 旧名称（VALO NEXUS）から

ORIVEIL was previously released as "VALO NEXUS". On first launch, ORIVEIL copies your data from `%APPDATA%\VALO NEXUS` to `%APPDATA%\ORIVEIL`. The old folder is not deleted.

初回起動時に旧データをコピーして引き継ぎます。旧フォルダは削除しません。

## Operator / 運営

**ORIVEIL Development**

Contact / お問い合わせ: support@oriveil.app

---

ORIVEIL isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing Riot Games properties. Riot Games, and all associated properties are trademarks or registered trademarks of Riot Games, Inc.
