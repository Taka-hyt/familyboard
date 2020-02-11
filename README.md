# FamilyBoard 
アプリケーション名  

## コンセプト  
夫婦で共有するTODOアプリケーション  

## 目標  
TODOアプリとしてリリースする

## 使用する技術・ツール
- Nuxt.js  
- AntDesign  

## 機能一覧
- TODO一覧表示
- TODO投稿
- TODO削除
- TODO編集
- カテゴリー一覧
- ドロワー
- ダイアログ

## 画面一覧
- ログイン画面
  2人で使えるように管理画面を2画面作成することで切り分ける。ユーザー名、E-Mail、パスワード、ログイン、Google API
- TODO一覧、投稿、完了画面
- TODO編集、削除画面
- 完了TODO表示画面
- ドロワー画面
  ドロワーの中にカテゴリー一覧、新しいカテゴリを追加を表示

## コンポーネント  
- ボタン
- ハンバーガーメニュー
- ドロワー
- 入力フォーム
- カード

## 必要な関数  
- addTodo  
- deleteTodo
- editTodo
- doneTodo
- addCategory
- getTodoList
- getCategory
- getDoneTodo
- openDrawer
- openDialog 
- drawerOpener
- dialogOpener
- validRequired
- validDuplication
- validMinLength
- validMaxLength
- validEmail
- validPassword
- getErrorMsg
