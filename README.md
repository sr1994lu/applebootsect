## applebootsect
### introduction
Boot Camp アシスタント ("/Applications/Utilities/Boot Camp Assistant.app") に頼らずにMac OS X上でブータブルなWindows 10インストール用USBフラッシュドライブを作成するのは難しい。ブートストラップローダーを準備するのが面倒なためである。
### what is this
アップル製のブートローダーをブートセクターに書き込むユーティリティ
### how to

`applebootsect /dev/disk_media /dev/disk_volume`

1. disk_mediaは MBR 書き込み先デバイス
2. ディスク全体に対応するデバイスファイル名を指定する
3. disk_volumeは PBR 書き込み先デバイス
4. FAT32パーティションに対応するデバイスファイル名を指定する
