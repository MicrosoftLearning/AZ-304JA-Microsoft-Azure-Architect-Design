---
title: オンライン ホステッド インストラクション
permalink: index.html
layout: home
---

# コンテンツ ディレクトリ

ラボを完了するために必要なファイルは、 [ここで](https://github.com/MicrosoftLearning/AZ-304JA-Microsoft-Azure-Architect-Design/archive/master.zip)ダウンロードすることができます

各ラボの演習とデモへのハイパーリンクを以下に一覧表示します。

## ラボ

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| モジュール | ラボ |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

