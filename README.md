Flasky
======

This repository contains the source code examples for the second edition of my O'Reilly book [Flask Web Development](http://www.flaskbook.com).

The commits and tags in this repository were carefully created to match the sequence in which concepts are presented in the book. Please read the section titled "How to Work with the Example Code" in the book's preface for instructions.

For Readers of the First Edition of the Book
--------------------------------------------

The code examples for the first edition of the book were moved to a different repository: [https://github.com/miguelgrinberg/flasky-first-edition](https://github.com/miguelgrinberg/flasky-first-edition).


pipenvとPipfile.lockの作成まで
----------------------------

git clone https://github.com/norabal/flasky.git
pipenv install --python 3.6
pipenv install -r requirements/common.txt
pipenv install -r --dev requirements/dev.txt  # dev.txt内のcommon.txt読み込みを削除してから実行
pipenv install -r requirements/dev.txt --dev

gmailの設定
----------

送信するgmailアカウントにログインして、「セキュリティ」の項目から二段階認証を設定し、かつ、アプリパスワードを発行する。

環境変数として以下を登録。
- MAIL_USERNAMEはgmailのメルアド。
- MAIL_PASSWORDはアプリパスワード。

