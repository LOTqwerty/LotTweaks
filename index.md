# LotTweaks for Minecraft 1.12.2

LotTweaks は建築補助を目的としたクリエイティブモード向けMODです。

"LotTweaks" adds some tweaks for builders to increase productivity in Creative mode.

## 追加されるキー / Keys

### 'Ex Pick' key (Client)

- 長距離のPick (100ブロック以上)
/ Extended 'Pick block' (up to 100+ blocks away)
- 長押し + マウスホイール で隣接ブロックのPickも可能です。
/ long press + wheel to pick 'near' blocks

### 'Rotate' key (Client)

- 手持ちブロックを同じグループの別ブロックで置き換えます。
/ swap the current block to next block in the same block-group.
- グループはconfigで設定するか、 `/lottweaks add` コマンド（下記）で追加します。
/ block-groups can be determined by a config or added by `/lottweaks add` command.
- 操作方法: 長押し + マウスホイール
/ long press + wheel

![](rotate.gif)

### 'Replace' key (Client + **Server** )

- 視線の先にあるブロックを手持ちブロックで置換します。
- マルチでこの機能を使うには、 **サーバ側にもLotTweaksの導入が必要** です。

## コマンド / Commands

### `/lottweaks add` command (Client)

- ホットバー内のブロックを左から順にグループとして登録します。
- 最大で9ブロックまでを一度に登録できます。
- `add` は省略できません。
- 実験的機能のため、Configファイルのバックアップを推奨します。
- [How to use](https://twitter.com/LOTqwerty/status/1312584389675552768)

## Configについて / About Config

- REPLACE_RANGE : Replace の最大長さ。クライアント/サーバのConfigの短い方が適用されます。
- REPLACE_INTERVAL : Replace が連続実行されるまでの長押し時間。
- REQUIRE_OP_TO_USE_REPLACE : Replace の実行権限をOPに限定します。一般公開するサーバでは、 `true` にセットするか、MODごと無効化してから公開してください。 
- BLOCK_GROUPS : 下記

### ブロックグループ

- 1つのブロックは1つのグループのみに所属できます。複数グループには所属できません。
- アイテムは登録できません。
- configでは `ブロック名/メタ` の形式で、カンマ `,` 区切りで記述します。
- メタ0番の場合はメタを省略し、ブロック名のみで登録できます。

例: ガラスブロック(メタ0)、本棚(メタ0)、土(メタ1)を登録するときは、 `minecraft:glass,minecraft:bookshelf,minecraft:glass,minecraft:dirt/1`

## 導入方法 / How to install

Forge 1.12.2 - 14.23.5.2854 を導入後、modsフォルダに入れてください。 / Requires MinecraftForge 1.12.2 - 14.23.5.2854

## ダウンロード / Download

**必ず事前の&定期的なバックアップを実施してください。**

**本MODの使用またはその他の扱いによって生じるあらゆる事柄について、作者は責任を負わないものとします。**

[上記に同意の上、ダウンロードする / Accept the disclaimer above and download](https://drive.google.com/drive/folders/15P4FLZgDrP7vwP9E47XhJRwj71IVASuc)

## 更新履歴

1.1.3

- 公開

## よくある質問・あまりない質問 / FAQ

- Replaceだけ使えない

サーバ側に導入できていない可能性があります。確認してみてください。

- MODの追加ブロックで使えますか？

標準的なブロックであれば、Configに追加すれば動作するはずです。

動作しない or クラッシュするなら、そのMODには非対応です。

- マルチで使えますか？

Ex Pick と Rotate は、どのサーバでも使えるはずです。

Replace はForge系のサーバで、サーバにもLotTweaksが導入されている必要があります。

- サーバプラグインと同時に使えますか？

Sponge Forge などのサーバであれば使えるかもしれません。動作確認はしていませんが。

- Rotateの順番を変えたい

Configをいじってください。

- Configファイルが壊れた/初期化したい

Configファイルを削除してからMinecraftを起動すると、初期値で再生成されます。

- Configファイルを公開・配布していい？

どうぞ。Configファイル単体の公開や配布に制限はありません。

- 新しい/古い マイクラに対応して

古いバージョンには対応できません。もう開発環境が無いので...。

新しいバージョンは.... 気が向いたら作るかもしれません。

個人的要因・技術的要因が大きく影響するので、今はなんとも言えません。

- 紹介・リンク

リンクは現在のアドレスへお願いします。（ https://lotqwerty.github.io/LotTweaks/ ）

ドライブへの直接リンクはNGです。

- 投げ銭

サービス登録してないので...。

密林ギフト券 \300 を作者のDMに送って頂くと、作者のPC環境がアップグレードされるかもしれません。

