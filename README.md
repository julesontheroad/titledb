# titledb

## titles.US.en.json
If you are looking for titles.US.en.json, this file was deleted because it was blowing up the size of this repository.  titledb/titles.json is the exact same file as titles.US.en.json, and can be generated with https://github.com/blawar/nut using one of two ways:

### Easy method
```
rm titledb/titles.json
nut.py --import-region US --language en
```

### Harder method
do a one time setup of:
```
rm titledb
git clone https://github.com/blawar/titledb titledb
```

then every day run the following to update:
```
git -C titledb pull
nut.py -U --import-region US --language en
```


### Files
`{region}.{language}.json` - Mapped by nsuId

[`cheats.json`](cheats.json) - Mapped by titleId > buildId

[`cnmts.json`](cnmts.json) - Mapped by titleId

[`ncas.json`](ncas.json) - Mapped by NCA

[`titles.US.en.json`](titles.US.en.json) - Mapped by titleId, used for [Tinfoil](https://tinfoil.io/Download#download)

[`versions.json`](versions.json) - Mapped by titleId, includes version history


### Online-only titles

```
010025400AECE800|Fortnite
0100647003750800|ドラゴンクエストⅩ ベーシックパック
01005A100D16E800|荒野行動
01004C400CF96800|Dead by Daylight
010023900AEE0800|Paladins
01005A600C318800|SMITE
0100B9500D1B0800|Dauntless
0100F8600E21E800|Overwatch: Legendary Edition
01001A400C53A800|ドラゴンクエストライバルズ エース
0100FEE00A64E800|Warframe
0100BC200B99E800|Onigiri
0100D0200E97A800|Rogue Company
0100D1E00E972800|Warface
01005B000D786800|DC Universe™ Online
01000A400DA58800|棋士・藤井聡太の将棋トレーニング
0100CC400DDE8800|Realm Royale
01008C80122BE800|Skyforge
0100D9500FC66800|Apex Legends
010076C01015C800|Spellbreak
```
