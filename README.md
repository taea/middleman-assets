# Middleman::Assets

Middleman プロジェクト用の asset ファイル管理 gem 雛形 for Desiner。

## Usage

このプロジェクトを fork し愛用の CSS, JS, 画像, フォントをそれぞれのディレクトリに入れ管理することで Middleman のプロジェクトで呼び出すことが可能です。

1. github でこのプロジェクトを fork する
2. 手元に `git clone`
3. CSS 等 asset ファイルを配置
4. ファイルを追加し更新する場合には `lib/middleman-assets/version.rb` の `VERSION` の数字を変更
5. `git add` && `git commit`
6. 自分の github リポジトリに `git push`

これで用意は完了です。

Middleman のプロジェクトでは次のようの使用します。

    $ middleman init PROJECT
    $ cd PROJECT 
    $ vi Gemfile 

Gemfile の中に次の内容を追加します。

    gem "middleman-assets", :github => 'YOUR_GITHUB_ACCOUNT/middleman-assets'

    $ bundle install --path vendor/bundle 

これで Middleman の中から利用したいライブラリを呼び出すことができます。

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
