# VScodeExtension
VSCode Extensionの開発方法をドキュメントとして残しておきます。  

## Hello World
参考サイト：  
https://code.visualstudio.com/api/get-started/your-first-extension

【前提】  
* Node.js,npm,Gitがインストール済み  
```
バージョン最新のものにしておいた方がいいかも。
```
* VScodeのバージョンは1.64.0以上

1.  YeomanとVS Code Extension Generatorのインストール
```
npm install -g yo generator-code
```
linux環境だとsudo必要かも。  
2. プロジェクト作成  
```
yo code
```
3. 質問に回答  
? What type of extension do you want to create? New Extension (TypeScript)
? What's the name of your extension? HelloWorld
Press <Enter> to choose default for all options below ###

? What's the identifier of your extension? helloworld
? What's the description of your extension? LEAVE BLANK
? Initialize a git repository? Yes
? Bundle the source code with webpack? No
? Which package manager to use? npm

? Do you want to open the new folder with Visual Studio Code? Open with `code`  

4. F5キーを押下してて、コンパイル、実行  
5. 新しいウィンドウが開くので、そこでCtrl + Shift + P  
6. コマンドパレットにhello worldと入力して実行すると、画面右下にhello worldの通知が現れる。

## 実装、ビルド、パッケージング
https://zenn.dev/tomi/articles/2021-03-26-vscode-extension  
hello worldの実装解説と、ビルド方法、パッケージング化の方法は上記のサイト参照  

用意されているAPI一覧は以下サイトにまとめられている。  
https://code.visualstudio.com/api/references/vscode-api  
