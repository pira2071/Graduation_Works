## ■サービス概要
日付と一緒に名言がランダムで表示される、日めくりカレンダーアプリです。  
名言は、フィクション小説の登場人物のセリフから引用されます（実在する偉人の格言等は除外します）。  
デフォルトで搭載されている名言以外にも、おすすめの名言を投稿することができ、投稿された名言は、ユーザー間で共有され、日めくりカレンダーに表示される名言をカスタマイズすることができます。

## ■ このサービスへの思い・作りたい理由
アプリ作成の理由は次のとおりです。  
・日常生活の中でやる気や活力等が湧かない時に、名言を読むと励みになることが多いため。  
・個人的な事情ではあるが、自身の趣味が読書であり、読書家向けのアプリを作成したいと考えたため。  
・読書家が次に読む本を探すときの一助になればと思ったため（その作品を象徴するようなセリフやかっこいいセリフを”読書名言集”のようなサイトで見るとその本を読みたいと感じることが多い）。

## ■ ユーザー層について
ユーザー層は、読書が趣味の人又は日常生活の中で名言等でやる気を出したい人です。  
当該ユーザー層を対象にした理由は、自身の個人的な経験等に基づいています（読書が趣味であり、また、日常生活の中でやる気が出ない時に、名言を読んで活力を得ることが多い）。

## ■サービスの利用イメージ
本アプリでカレンダーをめくることで、ユーザーは、日付の確認とともに名言を読むことができます。  
前記のとおり、名言を読むことでやる気の向上に繋がるとともに、読書が趣味の人にとっては、次に読む本を発掘できる良い機会になると考えます。

## ■ ユーザーの獲得について
現状具体的な案はありませんが、まず、このアプリが通常の日めくりカレンダーではなく、「読書好きな人」又は「これから読書を趣味にしたい人」を対象にしているアプリであることをアプリ名やUIから分かるようにすることが最優先だと考えています。

## ■ サービスの差別化ポイント・推しポイント
類似のアプリとしては、シンプルな日めくりカレンダーアプリが複数存在します。  
めくるカレンダー用紙に、日付とともに名言を表示させること及び名言の内容を小説中のセリフに限定することで、差別化を図っています。

## ■ 機能候補
・会員登録、ログイン機能（２回目以降の自動ログイン機能含む）（MVP / （自動ログイン機能は、本リリース））  
・カレンダーをめくり・名言表示機能（なお、名言表示欄下部には、小説のタイトル、その著者名も表示する）（MVP）  
・名言投稿機能（自分の投稿した名言の変種機能含む/投稿された名言は「名言一覧（仮）」画面で閲覧可）（MVP）  
・名言お気に入り機能（投稿された名言等をお気に入りに追加する機能）（MVP）  
・名言検索機能（名言一覧から著者名や書籍のタイトル、キーワード部分検索などで、名言を検索できるようにする）（MVP）  
・カレンダーカスタマイズ機能（お気に入りした名言を、カレンダーに表示される名言に加えることができる）（本リリース）  
・通知機能（アプリを開いていない人にカレンダーめくりを勧める通知）（本リリース）  
・前日の日めくり用紙に戻る機能（本リリース）  
・年間を通して、すでにカレンダー中に表示された名言は、年が切り替わるまでは、表示されないようにする（なお、名言は、３６６日分はアプリ作成者の方で、デフォルトでデータベースに保存予定である）

## ■ 機能の実装方針予定
・通知機能については、AWSのAmazon EventBridge、AWS Lambda、Amazon SNSを用いて実装予定です。  
・使用済名言のカレンダーへの非表示機能は、モデル及びデータベース設計の中で対応する予定です。  
・使用済名言のカレンダーへの非表示を、年の切り替えとともにリセットする機能は、AWSのAmazon EventBridge、AWS Lambdaを用いて実装予定です。
