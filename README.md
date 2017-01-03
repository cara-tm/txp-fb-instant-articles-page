# txp-fb-instant-articles-page
A simple one page RSS layout for Facebook's Instant Articles integration into Textpattern CMS
##Prerequisites
You will need a facebook activated "Page" account, then to set your custom Textpattern RSS link into the "Publication Tools" from your facebook Page, at least 10 published articles within your website, then wait for crawler bots.

More infos: [here from the official fb developers docs.](https://developers.facebook.com/docs/instant-articles/publishing/setup-rss-feed)
##Page layout
No plugins, you only need Textpattern CMS ;)

Just copy/paste [this page layout](https://github.com/cara-tm/txp-fb-instant-articles-page/blob/master/page) into Textpattern and associate it to a section name (that will be your "facebook Instant articles" RSS link URL).
##Customization
###Choosing the articles section
By defaut articles will be extracted from the "articles" section. If you want to change, sets the "section" attribute into this line (comma separated sections list allowed): `<txp:article_custom section="articles" limit="10"`(limited articles number: 10).
###Frequences
Note: The RSS feed is last website modification date updated. 
###Copyright Date
The copyright dates starts from the website first installation year. If you want to change this year, remove this code `$start= date("Y", get_pref('sql_now_created'));` by this one: `$start = 'YYYY';` where "YYYY" is an integer (the year).

##Article's customization into facebook from the Instant Articles editor
[See the "How To" here.](https://developers.facebook.com/docs/instant-articles/guides/format-overview)
##Ressources
[Instant Articles dedicated Website](https://instantarticles.fb.com/).
[Cover markup from the official facebook developers docs](https://developers.facebook.com/docs/instant-articles/reference/cover).
