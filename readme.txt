=== wp-flickr-press ===
Contributors: tatsuya, alexanderovsov
Donate link: http://fukata.org/
Tags: images,flickr
Requires at least: 3.8
Tested up to: 4.9
Stable tag: 2.6.4

Flickr integration for wordpress plugin.

== Description ==

Flickr integration for wordpress plugin.

Latest source: http://github.com/fukata/wp-flickr-press/

Features

1. Insert flickr media in post.
2. Cache search results.
3. Default settings at insert flickr media.
4. Setting value a tag rel and class property.
5. Support the php safe mode.
6. Support post thumbnail.

Dependencies

1. php-curl http://php.net/manual/ja/book.curl.php

Issues

If you want to report bugs and wishes to find a following.

https://github.com/fukata/wp-flickr-press/issues

== Installation ==

1. Download the plugin, unpack it and upload the 'wp-flickr-press' folder to your wp-content/plugins directory.
2. To grant write access to wp-content/plugins/wp-flickr-press/cache.
3. Activate the plugin through the 'Plugins' menu in WordPress.
4. [Create Your Flickr App](http://www.flickr.com/services/apps/create/apply/ "Create Your Flickr App") and settings OAuth Callback URL. Default OAuth Callback URL is `http://"Your Blog Domain"/wp-admin/admin.php?action=wpfp_flickr_oauth_callback
5. Go to [Settings] -> [FlickrPress] to configure the options.

== Frequently Asked Questions ==

None

== Screenshots ==

1. Search
2. Insert Post
3. Setting config
4. FullScreen Writing
5. New UI 1
6. New UI 2

== Changelog ==

= 2.6.4 =
* Fix: Fix parse img tag.

= 2.6.3 =
* Feature: Change flikcr web endpoint http to https. Overwrite by NSID if not set path alias.

= 2.6.2 =
* Feature: Add Debug Mode.

= 2.6.1 =
* Feature: Add Sub Options of img tag. display `width` and `height` properties.

= 2.6.0 =
* Feature: Show debug information on settings page.

= 2.5.6 =
* Fix: PHPFlickr-Oauth(dependency library) fix https when use socket.

= 2.5.5 =
* Fix: Don't start session on frontend(fixed phpFlickr library).

= 2.5.4 =
* Feature: Add open wp-flickr-press media library shortcut button.

= 2.5.3 =
* Fix: fixed bug of PHPFlickr-OAuth library.

= 2.5.2 =
* Feature: Multiple insert mode on mobile.

= 2.5.1 =
* Fix: Show selection-info.

= 2.5.0 =
* Feature: Support mobile devic but only insert single image.

= 2.4.8 =
* Fix: Support WordPress v4.9.

= 2.4.7 =
* Fix: [url] tag to new UI.

= 2.4.6 =
* Fix: Support [description] tag to old UI.
* Add: Notice old UI.

= 2.4.5 =
* Fix: Use with WooCommerce.

= 2.4.4 =
* Fix: Use with WooCommerce.

= 2.4.3 =
* Change: change thumbnail size `sq` to `q`

= 2.4.2 =
* Fix: custom post type. https://github.com/fukata/wp-flickr-press/pull/35

= 2.4.1 =
* Fix: Fix flickr oauth signed api.

= 2.4.0 =
* Fix: Fix flickr oauth.
* Please get oauth token again can't use before got token.

= 2.3.8 =
* Fix: Update select2 to full version.

= 2.3.7 =
* Fix: Check extract thumbnail or not when call `the_post_thumbnail` function.

= 2.3.6 =
* Modified: Replace title to album title when search by photoset and slideshow on.

= 2.3.5 =
* Feature: Support embed slideshow in album.

= 2.3.4 =
* Fix: Reset album select field.

= 2.3.3 =
* Feature: Add search field for album select.

= 2.3.2 =
* Fix: Plugin, Author URL.

= 2.3.1 =
* Bugfix: Doesn't work on firefox.

= 2.3.0 =
* Feature: Add template variable `description`.

= 2.2.0 =
* Feature: Add Embed Option(Header, Footer, Slideshow).

= 2.1.0 =
* Feature(beta): Use flickr image to post thumbnail.

= 2.0.0 =
* Feature: Add new UI.

= 1.9.19 =
* Bugfix: Check curl support SSL.

= 1.9.18 =
* Bugfix: Syntax error.

= 1.9.17 =
* Feature: Support Flickr API SSL.

= 1.9.16 =
* Feature: Add Reset OAuth Token button.

= 1.9.15 =
* Bugfix: Support user alias when list mode.
* Feature: Add null keyword insert template.
* Feature: Support multiple insert and insert template when thumbnail mode.

= 1.9.14 =
* Bugfix: Display two buttons when certain conditions.
* Bugfix: Pager next link broken when search by photosets.

= 1.9.13 =
* Add embed player align parameter.

= 1.9.12 =
* Implemented embed player.

= 1.9.11 =
* Fixed design for WP 3.8.

= 1.9.9 =
* Add sizes Square 150, Small 320, Medium 800.

= 1.9.8 =
* Miss numbering.

= 1.9.7 =
* Fixed typo default image size.
* Support SSL.

= 1.9.6 =
* Corresponding to WordPress 3.5 and not support less than v3.5.

= 1.9.5 =
* Add language ro_RO.

= 1.9.4 =
* Bugfix form url search type list.

= 1.9.3 =
* Add description for Flickr App CallbackURL.

= 1.9.2 =
* Fixed bug doesn't work activation single site.

= 1.9.1 =
* Fixed readme.txt
* Add message languages file.

= 1.9.0 =
* Fixed plugins in symlinked directories.

= 1.8.0 =
* Fixed bug Use larger than selected size when selected photo size doesn't exists.
* Add image class property option.
* Add photo path alias option.

= 1.7.8 =
* Formatting tags insert photo thumbnail search type.
* Modified to also search to find pictures of otosets in private mode.

= 1.7.7 =
* Fixed bug html entities escape photo title at insert thumbnail search type.
* Fixed bug can not search private photo at list search type.

= 1.7.6 =
* Html entities escape photo title at insert thumbnail search type.

= 1.7.5 =
* Add title property a tag at insert photo.

= 1.7.4 =
* Change settings menu capability.

= 1.7.3 =
* flickr-gallery Fixed a bug when used with plug-ins.

= 1.7.2 =
* Fixed bug v3.3.

= 1.7.1 =
* Add check cache directory permission.

= 1.7.0 =
* Add insert flickr media button when writing fullscreen mode.

= 1.6.2 =
* Change photo window height 550px thumbnail search.

= 1.6.1 =
* Don't Use PHP Session.

= 1.6.0 =
* Add Default Link URL Type.
* Add Photo Size Medium 640.

= 1.5.1 =
* Fixed bug undefined variable.

= 1.5.0 =
* Add Default File URL Size.

= 1.4.0 =
* fixed bug use original size when not exists large size.
* add link property rel and class.

= 1.3.3 =
* Add large size photo. Use original size if don't large size.

= 1.3.2 =
* Fixed bug media_upload.js doesn't load post.php.

= 1.3.1 =
* Disabled cache jquery-flickr-client.

= 1.3.0 =
* Search(Thumbnail)時にOAuthトークンを利用したアクセスに対応

= 1.2.2 =
* 不要なconsole.logを削除

= 1.2.1 =
* メッセージが正常に表示されていなかったバグを修正

= 1.2.0 =
* 国際化(日本語)対応

= 1.1.1 =
* jqueryのflickrプラグイン内のconsole.logをコメントアウト

= 1.1.0 =
* 旧UIの速度改善

= 1.0.0 =
* 新UIを実装

= 0.9.0 =
* POSTで呼び出していた部分をGETに変更

= 0.8.0 =
* 画像個別に取得していたサイズ情報を取得しないように修正

= 0.7.1 =
* 特権管理者以外でも更新できるように修正

= 0.7.0 =
* クイック設定を追加

= 0.6.0 =
* 挿入順序を追加

= 0.5.0 =
* デフォルトのソート項目を追加

= 0.4.0 =
* 検索項目にソートを追加

= 0.3.0 =
* ユーザIDの取得方法を直入力からOAuth連携に修正
* 画像挿入時のテンプレートを追加

= 0.2.0 =
* photosetで検索した際に詳細URL内のownerが抜けていたバグを修正
* マルチサイトを適用した場合に、ページングが動作していなかったバグを修正

= 0.1.0 =
* 一括挿入機能を追加

= 0.0.7 =
* タグサジェスト機能を追加

= 0.0.6 =
* Photosetsのプルダウンが選択状態が維持されないバグを修正
* キャッシュクリア用のボタンを追加

= 0.0.5 =
* API KEY、API SECRET、USER IDを未設定チェックを追加

= 0.0.4 =
* 検索機能追加

= 0.0.1 =
* 初回リリース

== Upgrade Notice ==
