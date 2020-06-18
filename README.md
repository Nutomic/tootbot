This project has been moved to https://yerbamate.dev/nutomic/tootbot

# TootBot

A small python 3.x script to replicate tweets on a mastodon account.

The script only need mastodon login/pass to post toots.

It gets the tweets from RSS available at http://nitter.net, then does some cleanup on the content:
- twitter tracking links (t.co) are dereferenced
- twitter hosted pictures are retrieved and uploaded to mastodon

A sqlite database is used to keep track of tweets than have been tooted.

The script is simply called by a cron job and can run on any server (does not have to be on the mastodon instance server).
