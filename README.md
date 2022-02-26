# ExtraPlugin
5chでだけ晒していたやつとか、ニッチそうなのをいろいろまとめる

## カスタムパラメータについて
カスタムパラメータは1つのオブジェクトの中に全て記載する必要があります。

よって、下記のように記載することになります。

※ 外枠の`{}`については各種スクリプトファイルの例からは省略している場合があるので注意してください
```
{
  <スクリプトAのカスタムパラメータ>,
  <スクリプトBのカスタムパラメータ>,
  <スクリプトCのカスタムパラメータ>,
  ...
  <スクリプトZのカスタムパラメータ>
}
```

例えば、当リポジトリの中にある
`専用条件を無視して武器を装備できる機能`を持たせる場合、下記のようにカスタムパラメータを記載する事になります
```
{
  ignoreConditionWeaponId：10
}
```
さらに`クリティカルが出なくなる武器を設定する機能`も持たせたい場合は、
対象武器のカスタムパラメータに下記のように記載する事になります。
```
{
  ignoreConditionWeaponId：10,
  invalidCritical: true
}
```


## 参考URL
https://srpgstudio.com/developer/custom.html
