% Unzip4Winマニュアル  
%   
% 2019/10/03  


Unzip4winは、「固定の文字列と日付文字列を組み合わせる」というルールに従ったパスワードのついたZIPファイルを展開するツールです。

例：

* password20190222
* 20190222password
* pass20190222word
\

### 目次

1. [使い方](#usage)
1. [インストール（アップグレード）方法](#how_to_install)
    * [ショートカットを作成する](#shortcut)
    * [右クリックの「送る」に追加する](#sendto)
1. [Windows Defenderにブロックされた場合](#defender)

# 使い方 {#usage}

PC上のUnzip4Winのアプリケーションファイル（もしくはそのショートカット）へZIPファイルをDrag & Dropするだけで展開します。
[右クリックの「送る」に追加する](#sendto)を実施している場合は、ZIPファイルを右クリックしてunzip4winへ「送る」だけで展開も可能です。
展開後のファイルは、元のzipファイルと同じフォルダに保存されます。

![](images/win/usage.png)

当日から100日前までの日付についてパスワードが一致するまで試行を行い、その間にパスワードが一致した場合に展開します。
試行回数以内にパスワードが一致しない場合は展開に失敗します。


# インストール（アップグレード）方法 {#how_to_install}

入手したUnzip4Winのzipファイル（unzip4win_windows.zip）を適当なフォルダで展開します。
以下、 `マイドキュメント`配下に展開するものとして説明します。

1. 入手したzipファイル（`unzip4win_windows.zip`）をマイドキュメントに保存します。

    ![](images/win/install/01_download_zip.png)

1. 「`マイドキュメント`」の「`unzip4win_windows.zip`」をダブルクリックしてzipファイルの中に移動します。

    ![](images/win/install/02_into_zip.png)

1. ツールバー上の「`ファイルをすべて展開`」をクリックします。

    ![](images/win/install/03_unzip.png)

1. 「`圧縮（ZIP形式）フォルダーの展開`」ウィンドウが開くので、「`展開`」ボタンをクリックします。

    ![](images/win/install/04_unzip_dialog.png)
    
    * アップグレード時には「`ファイルのコピー`」ウィンドウが開くので「`コピーして置き換える`」を選択します。
    
    ![](images/win/install/05_upgrade.png)
    
1. 以上でインストール（アップグレード）は完了です。
\

### ショートカットを作成する {#shortcut}

本アプリケーションは、ショートカットを利用することでもZIPファイルの展開が可能です。
ここでは、Windowsのデスクトップにショートカットを作成する方法を説明します。

1. アプリケーションのあるフォルダ（`マイドキュメント - unzip4win_windows`）を開きます。
1. `unzip4win.exe`を右クリックしたままデスクトップまでドラッグします。
1. 「`ショートカットをここに作成`」を選択します。
1. 必要に応じてショートカットの名前を変更します。

    ![](images/win/shortcut/01_create_shortcut.png)
\

### 右クリックの「送る」に追加する {#sendto}

ファイルを右クリックした際に表示されるメニューの「送る」に追加することで、ZIPファイルを右クリックから展開することが可能になります。

1. Windowsのスタートメニューから「`ファイル名を指定して実行`」を開きます。
    * もしくは「`[Windows] + [R]`」のショートカットで「`ファイル名を指定して実行`」を開きます。
    
    ![](images/win/shortcut/02_exec_file_name.png)
    
1. 「ファイル名を指定して実行」の画面に「`shell:sendto`」と入力して「`OK`」ボタンをクリックします。

    ![](images/win/shortcut/03_shell_sendto.png)
    
1. エクスプローラーで「`SendTo`」フォルダが開くので、ここに`unzip4win.exe`のショートカットを追加します。
    * ショートカットの作成方法は[ショートカットを作成する](#shortcut)を参考にしてください。
    
    ![](images/win/shortcut/04_sendto_shortcut.png)
    
1. 必要に応じてショートカットの名前を変更します。
    * 変更した名前が「送る」のメニューに表示されます。画像では名前を「ZIP展開ツール」にしています。

    ![](images/win/shortcut/05_sendto_menu.png)


# Windows Defenderにブロックされた場合 {#defender}

Windows 10を使用している場合、インストール・アップデート後の初回起動時にWindows DefenderによってUnzip4Winの実行がブロックされることがあります。

![](images/win/defender/01_defender.png)

その場合には、「`詳細情報`」をクリックすることで「`実行`」することができます。

![](images/win/defender/02_execute.png)
