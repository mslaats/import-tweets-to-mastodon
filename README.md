# How to imports Tweets into Mastodon (e.g. https://framapiaf.org )

#### Ask twitter for a data export

Go [here](https://twitter.com/settings/your_twitter_data).

#### Request a data archive and look for `tweets.js` (`/data/tweets.js`) after unpacking the archive zip file.

#### Clone this repo and run

```
git clone git@github.com:FGRibreau/import-tweets-to-mastodon.git
cd import-tweets-to-mastodon
npm install
MASTODON_API_BASEPATH=https://mastodon-example.com MASTODON_API_KEY=YOUR_TOKEN TWITTER_TWEETJS_FILEPATH=/path/to/tweets.js node import.js
```

* `MASTODON_API_BASEPATH` is your social mastodon site e.g `MASTODON_API_BASEPATH=https://aus.socia`.

* `MASTODON_API_KEY` is *your access token* generated by creating a new application in `settings/applications` with selecting `read`, `write` and `follow`.

* `TWITTER_YEAR` you can also choose the year, e.g. `TWITTER_YEAR=2010`.

Tips: add the `DEBUG=*` environment variable for verbose output.

:tada:

#### Need help?

- This project is open-sourced as is. 
- I won't do support for free.
- If you really want support please consider [sponsoring me](https://github.com/sponsors/FGRibreau) :+1:
