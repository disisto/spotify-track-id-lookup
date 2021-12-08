<p align="center">
<a href="https://troubleshooting.tools/lookup/spotify/track/"><img src="https://troubleshooting.tools/assets/img/troubleshooting.tools/gh_logo.png" height="200"></a>
</p>

# Spotify Track ID Lookup 

Spotify Track ID Lookup by troubleshooting.tools resolves the entered Spotify Track ID to track assigned by Spotify. Helpful when you need troubleshoot single tracks and your logfile log only tracks by ID.

## Content

1.) [Web page](https://github.com/disisto/spotify-track-id-lookup#1-web-page)
<br>
2.) [Webhook](https://github.com/disisto/spotify-track-id-lookup#2-webhook)
<br>
3.) [Open Graph](https://github.com/disisto/spotify-track-id-lookup#3-open-graph)
<br>
4.) [OpenSearch](https://github.com/disisto/spotify-track-id-lookup#4-opensearch)
<br>
5.) [HTML search form](https://github.com/disisto/spotify-track-id-lookup#5-html-search-form)


## 1.) Web page

Look up a Spotify Track ID

<ol>
<li>Visit with a web browser https://troubleshooting.tools/lookup/spotify/track/</li>
<li>Enter a Spotify Track ID in the search form</li>
<li>Hit enter key or submit button</li>
</ol>

## 2.) Webhook

Beside the classic form input on the web page, the web page supports also webhooks. This possibility is ideal to share a link and guide the recipient directly to the results.

**URL:** **`https://troubleshooting.tools/lookup/spotify/track/`** `{spotify_track_id}` <br><br>
Example: `https://troubleshooting.tools/lookup/spotify/track/6sPOmDulFtLzfX25zICNrC`

## 3.) Open Graph

Sharing the Webhook link into a web page or app that support the Open Graph protocol gives the opportunity to share a small excerpt of the results, without that the recipient need to visit the webpage itself.

Examples

Slack:<br>
<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opengraph/slack.png" style="width: 50%; height: 50%">

Discord:<br>
<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opengraph/discord.png" style="width: 50%; height: 50%">

WhatsApp:<br>
<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opengraph/whatsapp.png" style="width: 50%; height: 50%">

Twitter:<br>
<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opengraph/twitter.png" style="width: 50%; height: 50%">


## 4.) OpenSearch

The browser integration of troubleshooting.tools allows to use the browser address bar as a search input field, when needed, without visiting the original web page before.

This function is called OpenSearch and works with Apple Safari, Microsoft Edge, Mozilla Firefox and Google Chrome. Before we can start using it, we have to setup our browser for this function. Here an example for Google Chrome:

At the top right, click More <img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opensearch/0_menu.jpg"> and then **Settings**.

<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opensearch/1_google_chrome_settings.jpg">

Under "Search engine," click **Manage search engines**.

<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opensearch/2_manage_search_settings.jpg">

To the right of "Other search engines," click **Add**.

<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opensearch/3_search_engine_settings.jpg">

Fill out the text fields as shown below and click **Add**.

<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opensearch/4_edit_search_engine.jpg" align="right">

**Search engine:**<br>
`Enter troubleshooting.tools or a name of your choice.`

**Keyword:**<br>
`Enter the character "t" or a keyword of your choice, to trigger later the search function.`

**URL with %s in place of query:**<br>
`https://troubleshooting.tools/lookup/spotify/track/%s`

<br><br><br><br><br>

The setup is complete. You are still able to continue to enter a URL in the address bar or any search terms that trigger a Google search.

<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opensearch/5_google_search_bar.jpg">

The new feature is, if you enter an "t" followed by a space, then you activate the troubleshooting.tools search.

<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opensearch/6_troubleshooting.tools_search_bar_a.jpg">

<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opensearch/7_troubleshooting.tools_search_bar_b.jpg">

This cause that Google Chrome address bar react like the search field on this website.

<img src="https://github.com/disisto/spotify-track-id-lookup/blob/main/img/opensearch/8_troubleshooting.tools_search_bar_c.jpg">

## 5.) HTML search form

To integrate the search bar into a different web page a few line are needed. The look and feel can be adjusted as desired.

```html
<form method="post" action="https://troubleshooting.tools/lookup/spotify/track/">
  <input type="text" name="TRACKID" placeholder="">
  <input type="submit" value="&#128269;">
</form>
```

---
This project is not affiliated with <a href="https://www.spotify.com/">Spotify</a>.<br>
All mentioned trademarks are the property of their respective owners.
