## Beatrice Trainer v2 rc.2 対応　Unofficial Simple WebUI colab版

### バージョン履歴
- **2026.09.05**：Hugging Face通信障害によるエラーに対応
- **2026.01.14**：colab版 暫定的リリース
<br>
<br>
#### プログラム概要
<br>
<br>
本プログラムは、AIボイスチェンジャー「Beatrice」用の学習キット「Beatrice Trainer」を簡単に導入出来るようにしWebUI機能を追加したものです。  
『Beatrice』と『Beatrice Trainer』に関する詳細は、以下のリンクをご確認ください

- [Beatrice 2 についてのゆるい説明など（公式の解説ページ）](https://prj-beatrice.notion.site/Beatrice-2-266fb3c9fba480e8a0e3dc2f40d0bad3) 
- [Beatrice (AIボイスチェンジャー VST)](https://prj-beatrice.com/)
- [Beatrice Trainer (学習キット)](https://huggingface.co/fierce-cats/beatrice-trainer) 


### 注意！！！
こちらは公式リリースとは無関係の非公式プログラムです。 
WebUIに関する質問以外にはお答えすることは出来ません。また、現バージョンのみの対応となっており、公式のアップデートにより使用不可能になる可能性があります。

---
  
### 使い方
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/niel-blue/niel-blue-beatrice-trainer-webui-colab/blob/main/Beatrice_Trainer_unoffisial_webui_colab_260905.ipynb)  
使用するGoogleアカウントでインした状態で上記のリンク先を開き、自身のドライブ内にコピーしてください。
基本的にローカルのwebui版と使い方は同じです。  
<br>
本プログラムはGoogle Drive内の音声ファイルにアクセスしたり、ドライブ内に生成結果を出力する都合上、Google Driveへのアクセスの許可を求めます。
生成されたモデルデータはそれなりに大きな容量になることがあります。最低でも5GB前後の空き容量を確保しておいてください。  
<br>
Beatriceは1モデル内で『複数話者をまとめて学習』が基本設計となっています（※もちろん一人だけでも可能）  
音声ファイルはGoogle Drive内に以下のような配置にしておいてください。  
この例の場合はdataset_1という名前のモデル名になり、その中から話者を選ぶという構成になります。  
（※各名前はモデル作成後に変更可能です）  
<br>
例）  
My Drive/  
　　├── dataset_1/  
　　│　　　├── speaker1/  
　　│　　　│　　　├── audio1.wav  
　　│　　　│　　　└── audio2.flac  
　　│　　　└── speaker2/  
　　│　　　　　　　└── audio1.wav  
　　└── output/
<br>
<br>
dataset_1 をデータフォルダのパス、outputを出力先として指定することになります。  
<br>
<img width="710" height="223" alt="inout" src="https://github.com/user-attachments/assets/5454f4b2-87c8-4daa-bc2d-ab0568b3a813" />
<br>
<br>
音声ファイルが数秒ずつの複数のファイル構成になっていたり長尺音声ファイルだった場合は事前処理で無音削除・指定の長さにスライスすることが出来ます。処理はサーバーのローカルドライブにコピーされてから行われるのでドライブ上に書き込みなどは行いません。  
<br>
<br>
※注意！  
パス入力時、大文字小文字も正確に入力してください。またフォルダ階層を指定する時は\ではなく/を使用してください。  
無料枠の場合はおおよそ10000stepsほどでタイムアップになる可能性があります。セーブのインターバルは小さい値にすることをオススメします。
  
---
  
  
## ライセンス
このプロジェクトはMITライセンスのもとで公開されています。詳細は[LICENSE](LICENSE)をご覧ください。

## 免責事項
このプロジェクトは「Beatrice Trainer」の公式リリースではなく、非公式のカスタマイズツールです。  
使用に関しては自己責任でお願い致します。

