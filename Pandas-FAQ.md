# Pandas FAQ

## pandas columns, shape, info(), describe()
* [ゆるふわPandasチートシート - Qiita](https://qiita.com/tanemaki/items/2ed05e258ef4c9e6caac)
* [Python Pandasでのデータ操作の初歩まとめ − 前半：データ作成＆操作編 - Qiita](https://qiita.com/hik0107/items/d991cc44c2d1778bb82e)
* [Pandas のデータフレームを確認する – Python でデータサイエンス](https://pythondatascience.plavox.info/pandas/%E3%83%87%E3%83%BC%E3%82%BF%E3%83%95%E3%83%AC%E3%83%BC%E3%83%A0%E3%82%92%E7%A2%BA%E8%AA%8D)

---

## pandas dtype 変更
* [Pandas DataFrameのカラムのdtype変更 | Jun SASAKI Laboratory 東京大学 佐々木淳 研究室（柏キャンパス）](http://estuarine.jp/2016/07/pandas-dataframe_column_dtype/)
* [pandasのDataFrameの複数列を同時にastypeで型変換 - Qiita](https://qiita.com/driller/items/af1369a5c0fc2ec61af3)
* [pandasでデータを読み込むときに気を付けること(dtypeの指定) - Qiita](https://qiita.com/haru1977/items/53c582eb9e264ccf8574)

---

## [nkmk note](https://note.nkmk.me/)
## pandas 列 特定の値を置き換える

* [pythonで列データの文字列置換 | NEHAN](http://nehan.io/blog/python-data-transform/id-17)

    ```
    ## data1のeducation列データの'-'を'_'に置換する
    data1['education'] = data1['education'].str.replace('-', '_')
    ```

* [pandas.DataFrame, Seriesの要素の値を置換するreplace | Python / note.nkmk.me](https://note.nkmk.me/python-pandas-replace/)
    ```
    df.replace('CA', 'California')
    ```

    ```
    df.replace('(.*)li(.*)', r'\1LI\2', regex=True)
    ```

    ```
    df['name'] = df['name'].str.replace('li', 'LI')
    ```

* [pandasで欠損値NaNを除外（削除）・置換（穴埋め）する | Python / note.nkmk.me](https://note.nkmk.me/python-pandas-nan-dropna-fillna/)

    ```
    df.fillna({'name': 'XXX', 'age': 20, 'point': 0})
    ```

* [<Python, pandas> 文字列の置換 - ねこゆきのメモ](http://nekoyukimmm.hatenablog.com/entry/2016/11/11/144255)

### YouTube
* [How do I handle missing values in pandas?](https://youtu.be/fCMrO_VzeL8)  
17,864 views, 14:27

## pandas.DataFrame, Seriesのインデックスを振り直す
* [pandas.DataFrame, Seriesのインデックスを振り直すreset_index | Python / note.nkmk.me](https://note.nkmk.me/python-pandas-reset-index/)

## pandas index starting from one
* [python - Start index at 1 when writing Pandas DataFrame to CSV - Stack Overflow](https://stackoverflow.com/questions/20167930/start-index-at-1-when-writing-pandas-dataframe-to-csv)
    ```
    result.index += 1
    ```
