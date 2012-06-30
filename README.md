# deTwitter

This crazy idea got started from a retweet made by [@aral](https://twitter.com/aral), of a
tweet made by [@mattgemmel](https://twitter.com/mattgemmell) that linked to a 
[blog post that proposes the idea of a decentralized Twitter-like service](http://inessential.com/2012/06/29/matthew_on_twitter_restrictions)

## Crazy, step one
My proposition is that this is entirely within the realm of possibility, what I attempt to discover is the feasibility
and practicality of such a system.

## Inspiration
I'm thinking it might be possible to build this and hopefully make it somewhat tamper-proof by building it on a
shasum system similar to what Git uses, in particular in conjunction with signed tags that leverage GPG.
In addition by building it to function with a protocol similar to BitTorrent, it might be possible to distribute
status updates between all connected clients.

There are some immediate concerns that comes to mind, such as if there are few clients, each client might have to
be asked to store all recent (assuming we only want to persist status updates for a limited time) status updates.
This might not be such a big ask, as it's reasonable to assume that few clients means fewer status updates.
The algorithm should perhaps be tuned during initial testing to find a reasonable distribution factor that will
minimize, or hopefully remove, loss of status updates to due client connectivity (some form of self-adjusting
redundacy factor).