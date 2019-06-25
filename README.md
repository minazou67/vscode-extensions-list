# vscode-extensions-list

VS Code の拡張機能をインストールするためのリストです。  
拡張機能を同期するための拡張機能も存在しますが、GitHub へのアクセスが必要となります。  
このリストを使用すると GitHub アカウント不要で、拡張機能がインストール可能です。

## Environment

* Windows 10
* VSCode 1.30.2

## Usage

インストール端末の `%USERPROFILE%` フォルダにリストファイルを配備します。  
ターミナルから下記のコマンドを実行し、拡張機能をインストールします。

```powershell
cat vscode-extensions-list.txt |% { code --install-extension $_}
```

## Export

インストールされている拡張機能をリストファイル化する場合は、下記のコマンドを実行します。  
リストファイルは `%USERPROFILE%` フォルダに作成されます。

```powershell
code --list-extensions > vscode-extensions-list.txt
```
