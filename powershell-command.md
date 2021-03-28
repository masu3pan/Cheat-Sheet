# 1. powershellでよく使うコマンド集
powershellでよく使うコマンドを目的別にまとめました

- [1. powershellでよく使うコマンド集](#1-powershellでよく使うコマンド集)
  - [1.1. ファイルの一覧を取得する](#11-ファイルの一覧を取得する)
    - [1.1.1. 基本構文](#111-基本構文)
    - [1.1.2. 正規表現](#112-正規表現)
    - [1.1.3. ファイル出力](#113-ファイル出力)
    - [1.1.4. オプション](#114-オプション)
  - [1.2. 参考URL](#12-参考url)


## 1.1. ファイルの一覧を取得する

### 1.1.1. 基本構文
> Get-ChildItem -Path [folderpath]

### 1.1.2. 正規表現  
`folderpath`でワイルドカードで任意のファイルを指定することが可能
- C:\Test\*.txt
- C:\Test\*

### 1.1.3. ファイル出力
`> filename`を末尾につける

### 1.1.4. オプション
基本構文のあとに付与する  

| オプション | 説明                                   |
| ---------- | -------------------------------------- |
| -Name      | ファイル名のみ取得する                 |
| -Recurse   | 配下アイテムを再帰取得する             |
| -Force     | 隠しアイテムを含む                     |
| -Include   | 以降で指定する内容を取得対象に含める   |
| -Exclude   | 以降で指定する内容を取得対象に含めない |


## 1.2. 参考URL
- [マイクロソフト公式ドキュメント - Microsoft.PowerShell.Management](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/?view=powershell-7.1)