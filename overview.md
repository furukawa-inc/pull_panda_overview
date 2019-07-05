# 概要

**Pull Panda**

以下3つの機能を自動化するツール。

- Pull Reminders
- Pull Analytics
- Pull Assigner

## Pull Reminders

PR作成、コメントがされた等の粒度でslack通知をカスタマイズすることができる。
指定時間にPR review、reviewへの対応を促す仕組みを完備。

## Pull Analytics

PRの平均merge timeや修正量、各コントリビューターのコメント量などを一覧にする。
チームやリポジトリごとの取り組みが可視化、データを元に組織文化の改善材料にできる。

## Pull Assigner

PR reviewerが偏らないように自動的にコントリビューターをassignできる。

## slackのgithub連携との違い

通知レベルをチャンネルごとにではなくて、個人ごとにも設定できるのでカスタマイズしやすい。
reviewのreminderがあるのでreview依頼の手間が省ける。
review doneの連絡もいらない。

### カスタマイズ例

```
リマインダー機能(チャンネルへのリマインダー)

11:00と17:00の1日2回リマインダー at #android_pr
レビュー待ち、レビューコメント対応待ちの2条件で通知
PRは作成されて2時間以上たったものを通知
通知したくないPRには WIP ラベルをつける
リマインダー機能(個別DMへのリマインダー)

カスタマイズ推奨
開発スタイルに合わせておまかせ
自動アサイン機能(Automated review assignment)

Androidチームは CODEOWNER を利用しているため対応しない
Androidチームが増えたら対応を検討(2019年6月現在3名)
```

