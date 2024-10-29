# Solid Cache on 37signals

* Basecampは[fragment caching](https://guides.rubyonrails.org/caching_with_rails.html#fragment-caching)を多用しており、保存しているキャッシュのレコードが増えた≒キャッシュのヒット率があがり、結果全体としては性能改善したとのこと
* 結果、37sginalsとしては、運用コストは下がったし、性能もよくなったしとのこと
