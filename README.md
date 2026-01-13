## Beatrice Trainer v2 rc.0 対応　Unofficial Simple WebUI colab版

### バージョン履歴
- **2026.01.14**：colab版 暫定的リリース

#### プログラム概要

本プログラムは、AIボイスチェンジャー「Beatrice」用の学習キット「Beatrice Trainer」を簡単に導入出来るようにしWebUI機能を追加したものです。  
『Beatrice』と『Beatrice Trainer』に関する詳細は、以下のリンクをご確認ください

- [Beatrice (AIボイスチェンジャー VST)](https://prj-beatrice.com/)
- [Beatrice Trainer (学習キット)](https://huggingface.co/fierce-cats/beatrice-trainer) 


### 注意！！！
こちらは公式リリースとは無関係の非公式プログラムです。 
WebUIに関する質問以外にはお答えすることは出来ません。また、現バージョンのみの対応となっており、公式のアップデートにより使用不可能になる可能性があります。

---
  
### 使い方（仮  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/niel-blue/niel-blue-beatrice-trainer-webui-colab/blob/main/Beatrice_Trainer_unoffisial_webui_colab_0113.ipynb)  

    
基本的にはローカルのwebui版とだいたい同じです。  


  
本プログラムはGoogle Drive内の音声ファイルにアクセスしたり、ドライブ内に生成結果を出力する都合上、Google Driveへのアクセスの許可を求めます。
また、最低でも5GB前後の空き容量を確保しておいてください。  

  
音源ファイルは以下のような配置にしておいてください。  

  
例）  
マイドライブ/  
├── dataset_1/    ※このフォルダ名がモデル名になります  
│   ├── 話者1/  
│   │　　├── 音声ファイル1.wav  
│   │　　└── 音声ファイル2.flac  
│   └── 話者2/  
│　　　 └── 音声ファイル1.wav  
└── output/  

  
  
上記の場合、webui上では、dataset_1 をデータフォルダのパス、outputを出力先として指定することになります。  

  
---
  
  
## ライセンス
このプロジェクトはMITライセンスのもとで公開されています。詳細は[LICENSE](LICENSE)をご覧ください。

## 免責事項
このプロジェクトは「Beatrice Trainer」の公式リリースではなく、非公式のカスタマイズツールです。  
使用に関しては自己責任でお願い致します。

