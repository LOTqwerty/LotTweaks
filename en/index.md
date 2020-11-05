# LotTweaks

LotTweaks adds some tweaks for builders to increase productivity in Creative mode.

## Keys

### 'AdjustRange' key (Client + **Server** )

- Press to adjust the max distance of placing/breaking blocks.

### 'Rotate' key (Client)

- Press + wheel to swap the current block to the next block in the same block-group.
- Block-groups can be determined by a config or added by `/lottweaks add` command.

![](rotate.gif)

### 'Replace' key (Client + **Server** )

- Replace the block you're looking by the block in your main hand.

### 'Ex Pick' key (Client)

- Extended 'Pick block' (up to 100+ blocks away)
- Long press + wheel to pick 'near' blocks.

## Commands

### `/lottweaks add` (Client)

- Register blocks in your hotbar as a new block-group.
- This is an experimental feature.
- [How to use](https://twitter.com/LOTqwerty/status/1312584389675552768)

### `/lottweaks reload` (Client)

- Reload block-groups from config file.

## About Config

- REPLACE_RANGE : The range limitation of 'Replace'.
- REPLACE_INTERVAL : The interval of 'Replace'.
- REQUIRE_OP_TO_USE_REPLACE : Ristrict 'Replace' to OPs.
- BLOCK_GROUPS : v

### Block-groups

- 1 block cannot belong to multiple groups.
- Items cannot be registred.
- The format of config is `THE-BLOCK-NAME/META-VALUE` and the delimiter is `,` .
- If META-VALUE is omitted, META=0 will be used.

Sample:

`minecraft:glass,minecraft:bookshelf,minecraft:dirt/1`

## Installation

Requires MinecraftForge 1.12.2 - 14.23.5.2854

## Download

**必ず事前の&定期的なバックアップを実施してください。**

**本MODの使用またはその他の扱いによって生じるあらゆる事柄について、作者は責任を負わないものとします。**

[Accept the disclaimer above and download](https://drive.google.com/drive/folders/15P4FLZgDrP7vwP9E47XhJRwj71IVASuc)

## Change log

### 1.2.3

- Fix using 'Rotate' on MOD blocks generates missing texture items.

### 1.2.2

- Add 'AdjustRange' key.
- Add `/lottweaks reload` command.
- New config file for block-groups.

### 1.1.3

- (Initial version)

## FAQ

<!--
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

-->

- Can I distribute my block-group config file?

Yes.

<!--

- 新しい/古い マイクラに対応して

古いバージョンには対応できません。もう開発環境が無いので...。

新しいバージョンは.... 気が向いたら作るかもしれません。

個人的要因・技術的要因が大きく影響するので、今はなんとも言えません。

- 紹介・リンク

リンクは現在のアドレスへお願いします。（ https://lotqwerty.github.io/LotTweaks/ ）

ドライブへの直接リンクはNGです。

-->
