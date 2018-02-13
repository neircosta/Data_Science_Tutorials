### Basketball-Reference Scraping
#### October 2017

#### How Do I Transfer Tables to Markdown
1) Search for Table
2) Select 'Share & More' Drop-down Menu
3) Select 'Modify & Share Table'
4) Select REDDIT
5) Copy the table
6) Paste it into Markdown file

Example (Russell Westbrook Career Stats):

|Season|Age|Tm|Lg|Pos|G|GS|MP|FG|FGA|FG%|3P|3PA|3P%|2P|2PA|2P%|eFG%|FT|FTA|FT%|ORB|DRB|TRB|AST|STL|BLK|TOV|PF|PTS|
|:-|:-|:-|:-|:-|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|-:|
|2008-09|20|OKC|NBA|PG|82|65|32.5|5.3|13.4|.398|0.4|1.6|.271|4.9|11.8|.415|.414|4.3|5.2|.815|2.2|2.7|4.9|5.3|1.3|0.2|3.3|2.3|15.3|
|2009-10|21|OKC|NBA|PG|82|82|34.3|5.9|14.1|.418|0.3|1.3|.221|5.6|12.9|.438|.428|4.0|5.1|.780|1.7|3.1|4.9|8.0|1.3|0.4|3.3|2.5|16.1|
|2010-11|22|OKC|NBA|PG|82|82|34.7|7.5|17.0|.442|0.4|1.3|.330|7.1|15.7|.451|.454|6.5|7.7|.842|1.5|3.1|4.6|8.2|1.9|0.4|3.9|2.5|21.9|
|2011-12|23|OKC|NBA|PG|66|66|35.3|8.8|19.2|.457|0.9|3.0|.316|7.8|16.2|.482|.481|5.2|6.3|.823|1.5|3.1|4.6|5.5|1.7|0.3|3.6|2.2|23.6|
|2012-13|24|OKC|NBA|PG|82|82|34.9|8.2|18.7|.438|1.2|3.7|.323|7.0|15.1|.466|.470|5.6|7.0|.800|1.4|3.9|5.2|7.4|1.8|0.3|3.3|2.3|23.2|
|2013-14|25|OKC|NBA|PG|46|46|30.7|7.5|17.2|.437|1.5|4.7|.318|6.0|12.5|.482|.480|5.3|6.4|.826|1.2|4.5|5.7|6.9|1.9|0.2|3.8|2.3|21.8|
|2014-15|26|OKC|NBA|PG|67|67|34.4|9.4|22.0|.426|1.3|4.3|.299|8.1|17.7|.457|.455|8.1|9.8|.835|1.9|5.4|7.3|8.6|2.1|0.2|4.4|2.7|28.1|
|2015-16|27|OKC|NBA|PG|80|80|34.4|8.2|18.1|.454|1.3|4.3|.296|6.9|13.8|.503|.489|5.8|7.2|.812|1.8|6.0|7.8|10.4|2.0|0.3|4.3|2.5|23.5|
|2016-17|28|OKC|NBA|PG|81|81|34.6|10.2|24.0|.425|2.5|7.2|.343|7.7|16.8|.459|.476|8.8|10.4|.845|1.7|9.0|10.7|10.4|1.6|0.4|5.4|2.3|31.6|
|Career|||NBA||668|651|34.1|7.8|18.1|.433|1.1|3.4|.313|6.8|14.7|.461|.462|5.9|7.2|.823|1.7|4.5|6.2|7.9|1.7|0.3|3.9|2.4|22.7|

#### How Do I Scrape Tables To Python
1) Search for Table
2) Select 'Share & More' Drop-down Menu
3) Select 'Copy Link to Table to Clipboard'
4) Switch to python:
~~~
url = 'https://www.basketball-reference.com/players/w/westbru01.html#per_game::none'
table = pd.read_html(url)[0]
~~~
* Further Tutorial: https://www.youtube.com/watch?time_continue=3305&v=2RW9zSQF1Sk