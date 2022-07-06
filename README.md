# 自作ネームプレートの追加方法
### 1.このリポジトリを[Fork](https://github.com/tugaru1975/TOPNamePlates/fork)する
### 2.Forkしたリポジトリの`NamePlates`に自作したネームプレートスキンをアップロード
### 3.アップロードしたら`CustomNamePlates.json`にコードを追加する
```
        {
            "name": "題名",
            "author": "制作者名",
            "resource": "ネームプレートの画像名.png"
        },
```  
**※いらないコードは消してください**  
**※`,`を最後の行では削除してください**
#### コードの説明
`"name"` : ネームプレートの題名  
`"author"` : 制作者名  
`"resource"` : ネームプレート画像を決められる。  
### 4.TOPに対応させる
AmongUsファイルのデフォルト状態なら  
Steam : `C:\Program Files (x86)\Steam\steamapps\common\Among Us`  
Epic : `C:\Program Files (x86)\Epic Games\AmongUs`にある、  
`BepInEx` > `config` > `com.tugaru.TownOfPlus.cfg`を開きます。  
**開けない場合は`.cfg`を`.txt`にします。**  
次に下にスクロールしていくと
```
[NamePlateURL]

# Setting type: String
# Default value: https://raw.githubusercontent.com/tugaru1975/TOPNamePlates/master,https://raw.githubusercontent.com/ユーザー名/プロジェクト名/master
NamePlateURL = https://raw.githubusercontent.com/tugaru1975/TOPNamePlates/master,https://raw.githubusercontent.com/ユーザー名/プロジェクト名/master
```  
という部分があるので`/ユーザー名/`と`/プロジェクト名/`の部分をそれぞれ自身のgithubユーザー名とプロジェクト名(デフォルトは`TOPNamePlates`)にしてください。  
**`.txt`にしている場合は`.cfg`に戻してください。**  
そしてAmongUsを開いて導入されていたら完了です。
### 5(任意).TOPでの実装
自身のプロジェクトをこのプロジェクトにプルーリクエストしていただければTOPの方で実装いたします。  
**オリジナルのネームプレートを削除している場合は元に戻してからプルリクしていただけると嬉しいです。**
