# `アプリケーションのコンポーネントで、ハンドルされていない例外が発生しました。`という警告ウィンドウが表示される
---

ウィンドウ下部の`詳細`ボタンをクリックして表示される
```cs
Just-In-Time (JIT) デバッグを呼び出すための詳細については、
ダイアログ ボックスではなく、このメッセージの最後を参照してください。

************** 例外テキスト **************
```
以降のメッセージ内容にて、エラー内容の特定が可能です。

1. メッセージが以下の場合
    ```cs
    Just-In-Time (JIT) デバッグを呼び出すための詳細については、
    ダイアログ ボックスではなく、このメッセージの最後を参照してください。

    ************** 例外テキスト **************
    System.ArgumentOutOfRangeException: インデックスが範囲を超えています。負でない値で、コレクションのサイズよりも小さくなければなりません。
    パラメーター名:index
    場所 System.ThrowHelper.ThrowArgumentOutOfRangeException(ExceptionArgument argument, ExceptionResource resource)
    場所 System.Collections.Generic.List`1.get_Item(Int32 index)
    場所 InstantVtuber_2.FormMain.KeyTextChange()
    場所 InstantVtuber_2.FormMain.FormMain_Load(Object sender, EventArgs e)
    場所 System.Windows.Forms.Form.OnLoad(EventArgs e)
    場所 System.Windows.Forms.Form.OnCreateControl()
    場所 System.Windows.Forms.Control.CreateControl(Boolean fIgnoreVisible)
    場所 System.Windows.Forms.Control.CreateControl()
    場所 System.Windows.Forms.Control.WmShowWindow(Message& m)
    場所 System.Windows.Forms.Control.WndProc(Message& m)
    場所 System.Windows.Forms.Form.WmShowWindow(Message& m)
    場所 System.Windows.Forms.NativeWindow.Callback(IntPtr hWnd, Int32 msg, IntPtr wparam, IntPtr lparam)
    ```

    + 以下のファイルが破損している可能性があります。
        ```sh
        C:\InstantV_2\Setting\keymouse.csv
        C:\InstantV_2\Setting\shortcuts.csv
        ```
    + こちらからファイルをダウンロードし[^1]、同じ場所に再配置してください。
        + [keymouse.csv](https://raw.githubusercontent.com/96ENU-kuroinu/Vtuber2-md/main/document/csv/keymouse.csv)
        + [shortcuts.csv](https://raw.githubusercontent.com/96ENU-kuroinu/Vtuber2-md/main/document/csv/shortcuts.csv)

---
+ [だれでもVtuber QA 目次ページに戻る](index_vtuber2_qa.md)
+ [だれでもVtuber 目次ページに戻る](index_vtuber2.md)
+ [トップページに戻る](index_top.md#falhong-cha)

[^1]: `名前を付けてリンク先を保存`を選択してください。