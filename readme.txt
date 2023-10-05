ロム魂(256in1)のファームウェアです。
最大256のROMファイルをロム魂のフラッシュメモリに格納する事が出来ます。
ファイル格納用のフラッシュメモリ領域は4Mバイト弱です。

対応ファイル形式
* 各種ROMファイル
  非メガROM、ASCII8Kマッパー、ASCII16Kマッパー、KONAMIマッパー、R-TYPEマッパーに対応

使用法

1. 256in1ファームウェアファイルを作成します。

256in1に含めたいROMファイル(1～256ファイル)を用意し、以下の形式の名前にリネームします。

<NAME>.<MAPPER>.rom

<NAME>=任意の名前
この名前はゲーム選択メニューに表示されます。16文字を超える部分はメニューに表示されません。

<MAPPER>=ROMのマッパー形式(normal, ascii8k, ascii16k, konami, rtype の何れか)
* normal: 非メガROM
* ascii8k: メガROM ASCII8Kマッパー
* ascii16k: メガROM ASCII16Kマッパー
* konami: メガROM konamiマッパー
* rtype: メガROM R-TYPEマッパー

例:
1942.ascii8k.rom
Gradius.konami.rom
R-Type.rtype.rom
Super Pierrot.ascii16k.rom
Thexder.normal.rom

上記ROMファイルと256in1.exeを同じディレクトリにおいて256in1.exeを実行します。
コマンドプロンプトで実行すると以下のようなメッセージが出ます。
(ダブルクリックによる実行でも構いません)

～ ピーガー伝説のロム魂(256in1)ツール ～
[000] mapper:02 offset:00001902 name:1942
[001] mapper:04 offset:00021902 name:Gradius
[002] mapper:05 offset:00041902 name:R-Type
[003] mapper:03 offset:000a1902 name:Super Pierrot
[004] mapper:01 offset:000c1902 name:Thexder
使用領域: 830kB
空き領域: 3265kB

同ディレクトリに作成される256in1.uf2というファイルが256in1ファームウェアファイルです。

2. MSXに刺さっていない状態のロム魂をブートモードでPCに接続します。

ロム魂の裏面のBOOTSELボタン(穴の奥にボタンがあります)を押しながらPCとUSB接続して下さい。
接続が成功するとドライブが認識されます。

3. ロム魂に1で作成した256in1.uf2ファイルを書き込みします。

2で認識されたドライブに256in1.uf2をドラッグアンドドロップ(コピー)します。
コピーが完了するとドライブが見えなくなります。

4. 書込みが終わったらPCから外して完了

注意：PCとの接続中はバスバッファの入力がフロート状態となります。
あまり良い状態ではないので長時間のPC接続は避けてください。

5. ゲーム起動方法

上下左右キーでゲームを選択してリーターンキー又はスペースキーでゲーム起動です。

上: 1戻る
下: 1進む
左: 16戻る
右: 16進む
