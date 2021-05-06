<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Social</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__html"><h1 id="hardware-hub-to-social-media"># Hardware Hub to Social Media</h1>
<p>Posts a product from the website (<a href="https://zed.exioite.com">https://zed.exioite.com</a>) to the twitter page (<a href="https://twitter.com/hub_hardware">https://twitter.com/hub_hardware</a>) and the Instagram page (<a href="https://www.instagram.com/hardware__hub/">https://www.instagram.com/hardware__hub/</a>)</p>
<h2 id="goal">Goal</h2>
<p>Semi-Automate the social media pages of the website to market the site without needing much human supervision</p>
<h2 id="technologies">Technologies</h2>
<p>-<strong>Tweet Invi:</strong> Post to a twitter page and read tweets programmatically.</p>
<blockquote>
<p><a href="https://github.com/linvi/tweetinvi">https://github.com/linvi/tweetinvi</a></p>
</blockquote>
<p>-<strong>Instagram API Sharper:</strong> Post to a Instagram page and read Instagram posts programmatically.</p>
<blockquote>
<p><a href="https://github.com/ramtinak/InstagramApiSharp/">https://github.com/ramtinak/InstagramApiSharp/</a></p>
</blockquote>
<p>-SQL: Database Storage to store a list of posts to be posted throughout the week</p>
<h2 id="procedure">Procedure</h2>
<ol>
<li><strong>GetNextID</strong>();</li>
</ol>
<ul>
<li>Reads the SQL Posts table and grabs the ID of the product that needs to posted that day.</li>
</ul>
<ol start="2">
<li><strong>TwitterPost</strong>(ID);</li>
</ol>
<ul>
<li>Grabs the data of the product by the ID, constructs a tweet, and posts the tweet</li>
</ul>
<ol start="3">
<li><strong>InstagramPost</strong>(ID);</li>
</ol>
<ul>
<li>Grabs the data of the product by the ID, constructs a post, and posts the post to Instagram</li>
</ul>
<h2 id="improvements">Improvements</h2>
<ul>
<li>Find a faster way to automatically run this program at 4:00 pm every day because sometimes I get busy and forget.</li>
</ul>
</div>
</body>

</html>
