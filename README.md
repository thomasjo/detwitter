# deTwitter
This crazy idea got sparked by a [blog post][1] that proposes the idea of a
decentralized Twitter-like service, which made its way to me thanks to
[@aral](https://twitter.com/aral) and
[@mattgemmel](https://twitter.com/mattgemmell).


## Crazy? Maybe...
My proposition is that this is entirely within the realm of possibility.
What I intend to discover is the feasibility and practicality of such a
system.


## Some initial thoughts
I'm thinking it might be possible to build this and hopefully make it
somewhat tamper-proof by building it on a shasum system similar to what Git
uses, in particular in conjunction with its signed tags that leverage GPG.

In addition by building it to function with a protocol similar to BitTorrent
without trackers, it might be possible to distribute status updates between
all connected clients. Essentially some form of naked P2P.

There are some immediate concerns that come to mind with a decentralized P2P
approach, such as if there are few clients, each client might have tobe asked
to store all recent (assuming we only want to persist status updates for a
limited time) status updates. This might not be such a big ask however, as
it's reasonable to assume that few clients means fewer status updates.
The algorithm should perhaps be tuned during initial testing to find a
reasonable distribution factor that will minimize, or hopefully eliminate,
loss of status updates to due client connectivity (some form of
self-adjusting redundacy factor).

In addition, how is discovery supposed to work? How do we make sure this
works behind a firewall, router with NAT and similar?


## Resources
- [Paper describing and comparing Gnutella and Freenet][2]
- [The original Freenet paper][3]
- [Distributed routing as employed in Freenet][4]
- [The Dark Freenet][5]


[1]: http://inessential.com/2012/06/29/matthew_on_twitter_restrictions
[2]: http://www.sysdesign.ca/archive/berkes_gnutella_freenet.pdf
[3]: https://freenetproject.org/papers/ddisrs.pdf
[4]: https://freenetproject.org/papers/swroute.pdf
[5]: https://freenetproject.org/papers/freenet-0.7.5-paper.pdf
