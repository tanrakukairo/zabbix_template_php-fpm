# zabbix_template_php-fpm

phpfpm Template for Zabbix ~> 3.4.

Necessary "Dependent Item". Put userparameter_phpfpm.conf in Include-UserParameter's Directory.

Necessary phpfpm_status.

- ZABBIX 3.4用 php-fpmのテンプレートです。
- UserParameterのワインライナーでphpfpm_statusをで取ってきて、依存アイテムで各値を入れてます。
- phpfpm_status?jsonでJSONがそのまま出ますけど、キーにスペースが入ってて依存アイテムが上手く取れないので、スペースをアンダースコアに変えてるだけです。
- phpfpm_statusの取り方は各自適当に。Nginx経由のconf置いておきます。
- FreeBSD11/CentOS7.1以上で動きます。

このテンプレートはMIT Licenseです。
