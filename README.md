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
| `ORIVEIL-Setup-1.1.2.exe` | Installer (per-user, no admin rights) / インストーラー（管理者権限不要） | 117 MB |
| `ORIVEIL-Portable-1.1.2.exe` | Portable (no installation) / ポータブル版（インストール不要） | 371 MB |
| `ORIVEIL-1.1.2-SHA256SUMS.txt` | SHA-256 checksums / チェックサム | — |

Requirements / 動作環境: Windows 10 / 11 (64-bit)

### Verify the download / ダウンロードしたファイルの確認

```powershell
Get-FileHash .\ORIVEIL-Setup-1.1.2.exe -Algorithm SHA256
Get-FileHash .\ORIVEIL-Portable-1.1.2.exe -Algorithm SHA256
```

Compare the result with `ORIVEIL-1.1.2-SHA256SUMS.txt`.

表示された値がチェックサムファイルと一致することを確認してください。

The files are not code-signed yet, so Windows may show “Windows protected your PC” when you open the downloaded file, with the publisher shown as “Unknown publisher” (this is because the file is unsigned, not because it is damaged). Make sure you downloaded it from https://oriveil.app or this repository and that its SHA-256 matches the checksum file, then choose “More info” → “Run anyway”. If it does not match, do not run it — delete it.

配布ファイルにはまだコード署名がないため、ダウンロードしたファイルを開くと「Windows によって PC が保護されました」と表示されることがあります。このとき発行元は「不明な発行元」と表示されます（署名がないためで、ファイルの異常ではありません）。ダウンロード元が https://oriveil.app またはこのリポジトリであることと、SHA-256 がチェックサムファイルと一致することを確認してから、「詳細情報」→「実行」を選んでください。一致しない場合は実行せずに削除してください。

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
