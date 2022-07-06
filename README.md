# 自作バイザーの追加方法
### 1.このリポジトリを[Fork](https://github.com/tugaru1975/TOPVisors/fork)する
### 2.Forkしたリポジトリの`Visors`に自作したバイザースキンをアップロード
### 3.アップロードしたら`CustomVisors.json`にコードを追加する
```
        {
            "name": "題名",
            "author": "制作者名",
            "resource": "バイザーの画像名.png"
        },
```  
**※いらないコードは消してください**  
**※`,`を最後の行では削除してください**
#### コードの説明
`"name"` : バイザーの題名  
`"author"` : 制作者名  
`"resource"` : バイザー画像を決められる。  
### 4.TOPに対応させる
AmongUsファイルのデフォルト状態なら  
Steam : `C:\Program Files (x86)\Steam\steamapps\common\Among Us`  
Epic : `C:\Program Files (x86)\Epic Games\AmongUs`にある、  
`BepInEx` > `config` > `com.tugaru.TownOfPlus.cfg`を開きます。  
**開けない場合は`.cfg`を`.txt`にします。**  
次に下にスクロールしていくと
```
[VisorURL]

# Setting type: String
# Default value: https://raw.githubusercontent.com/tugaru1975/TOPVisors/master,https://raw.githubusercontent.com/ユーザー名/プロジェクト名/master
VisorURL = https://raw.githubusercontent.com/tugaru1975/TOPVisors/master,https://raw.githubusercontent.com/ユーザー名/プロジェクト名/master
```  
という部分があるので`/ユーザー名/`と`/プロジェクト名/`の部分をそれぞれ自身のgithubユーザー名とプロジェクト名(デフォルトは`TOPVisors`)にしてください。  
**`.txt`にしている場合は`.cfg`に戻してください。**  
そしてAmongUsを開いて導入されていたら完了です。
### 5(任意).TOPでの実装
自身のプロジェクトをこのプロジェクトにプルーリクエストしていただければTOPの方で実装いたします。  
**オリジナルのバイザーを削除している場合は元に戻してからプルリクしていただけると嬉しいです。**
# 自作バイザーの試し方
AmongUsファイルのデフォルト状態なら  
Steam : `C:\Program Files (x86)\Steam\steamapps\common\Among Us`  
Epic : `C:\Program Files (x86)\Epic Games\AmongUs`にある、  
`TownOfPlus`>`SkinTest`のなかに自作したバイザー画像を入れると試すことが可能です。
