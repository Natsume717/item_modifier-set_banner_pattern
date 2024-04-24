# item_modifier-set_banner_pattern
item_modifierの1項目であるset_banner_patternに関するサンプルになります。

詳しくはブログ記事『[【マイクラ】set_banner_patternで旗の模様を適用【item_modifier】](https://natsumake.com/item_modifier-set_banner_pattern/)』を参考にしてください。

<h3>概要</h3>
バナーに模様を適用させることのできる、item_modifierの項目になります。<br>
また、バナー以外のアイテムに適用させた場合はtagは付与されますが、見た目に変化は起きません。

<h3>使い方</h3>

データパック導入後、ワールドに入り```/reload```と入力し実行してください。<br>
タラとサケのドロップアイテムが変更されているほか、```/reload```を実行すると計4種のアイテムが付与されます。

タラを倒すとダイヤモンドがドロップし、サケを倒すとバナーがドロップします。

どちらもset_banner_patternで模様が適用されており、バナーはその変化が明らかです。

ダイヤモンドについては、dataコマンドを使用することで適用されていることが分かります。<br>
※バナー以外のアイテムについては、見た目が変化しません。

調べるためのコマンドは、以下のようなものになります。<br>
※手に持っているアイテムのデータを調べるコマンドです。

```copy
/data get entity @s SelectedItem
```

また、itemコマンドでset_banner_patternを適用させる場合には、以下のようなコマンドでOKです。<br>
本データパックにおいては、手にバナーを持った状態で以下のコマンドを実行すれば、変化するようになっています。

```copy
/item modify entity @s weapon.mainhand sample:set_banner_pattern
```
