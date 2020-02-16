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
  
## メイン画面のコンポーネント
- Todo一覧を表示するナビゲーションメニュー
- Todoを表示するカード
- Todoを新しい日付順に表示する
- 重要なTodoを固定するクリップ
- クリックすると完了になるチェックボックス
- Todo入力フォーム
- Todo送信ボタン
- カテゴリ絞り込み検索ボタン
- 誰が投稿したのか分かるようにする色分け

## カテゴリ選択画面のコンポーネント  
- カテゴリ一覧
  - 買い物
  - 保育園
  - お出掛け
  - 完了済

- クローズボタン
- 色分け

## カテゴリ別Todoのコンポーネント
- Todoのカテゴリを表示するナビゲーションメニュー
- Todoを表示するカード
- Todoを新しい日付順に表示する
- 重要なTodoを固定するクリップ
- クリックすると完了になるチェックボックス
- Todo入力フォーム
- Todo送信ボタン
- カテゴリ絞り込み検索ボタン
- 誰が投稿したのか分かるようにする色分け

## 編集画面のコンポーネント
- ダイアログ
  - Todoタイトル
  - カテゴリ名のセレクトボックス
  - クローズボタン
  - 更新ボタン
  - 削除ボタン

## コンポーネント  
- Button
- Hamburger
- Drawer
- Inputform
- Card
- Dialog
- Navigation

## 必要な関数  
- TodoDao.add(todo)
- TodoDao.delete(todo.id)
- TodoDao.edit(todo)
- TodoDao.done(todo.id)
- TodoDao.undone(todo.id)
- TodoDao.clip(todo.id)
- TodoDao.unclip(todo.id)
- TodoDao.list(todo)
- TodoDao.date(todo.postDate)
- TodoDao.category(todo.categories[number])
- TodoDao.color(todo.color)


- Drawer.open
- Drawer.close

- Dialog.open
- Dialog.close

- Validator.checkrequired
- Validator.duplicated
- Validator.checkLength
- Validator.checkEmail
- Validator.checkPassword

- Message.provider.error 

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
- getErrorMsg(35分)

## 構造体  
Todo = {
  id: number,
  title: '',
  postDate: '',
  doneDate: '',
  isClip: false,
  done: fause,
  categories: [shopping, Nursery, goOut, done],
  color: [blue, red]
}

color = {
  id: '',
  colorData = ''
}

