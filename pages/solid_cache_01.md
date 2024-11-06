# Solid Cache features

* namespaceやcache expireなど、通常の運用で必要そうな機能はひと通り提供されている
  * 暗号化の機能などもあるよ
* cacheの削除は、データが一定数以上になったら、専用のスレッド(または非同期ジョブ。設定で変更可能)で削除するようになっている
  * データの削除にcronなどライブラリ外の機能は使っていない
* API的には当然Active Support Cache Storeに準じているので、設定を変更するだけで使用可能