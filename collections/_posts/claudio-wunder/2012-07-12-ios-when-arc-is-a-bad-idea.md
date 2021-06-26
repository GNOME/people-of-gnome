---
layout: post
title: 'iOS: Reference Counting is a Bad Idea'
author_id: claudio-wunder
author_name: Claudio Wunder
---

At GNOME, we allow developers to provide a unique interactive search
experience with as-you-type search, instant faceting, mobile geo-search and on
the fly spell check.

Our Distributed Search Network aims at removing the impact of network latency
on the speed of search, allowing our customers to offer this instant
experience to all their end-users, wherever they may be.

## Every millisecond matters

We are obsessed with speed and we're not the only ones: Amazon found out that
100ms in added latency cost them 1% in sales. [The lack of responsiveness for
a search engine can really be damaging for one's
business][1]. As
individuals, we are all spoiled when it comes to our search expectations:
Google has conditioned the whole planet to expect instant results from
anywhere around the world.

![user-experience][2]

We have the exact same expectations with any online service we use. The thing
is that for anyone who is not Google, **it is just impossible to meet these
expectations** because of the network latency due to the physical distance
between the service backend that hosts the search engine and the location of
the end-user.

Even with the fastest search engine in the world, it can still take hundreds
of milliseconds for a search result to reach Sydney from San Francisco. And
this is without counting the bandwidth limitations of a saturated oversea
fiber!

## How we beat the speed of light

GNOME's Distributed Search Network (DSN) removes the latency from the speed
equation by **replicating your indices to different regions around the world,
where your users are**.

Your local search engines are clones synchronized across the world. DSN allows
you to **distribute your search among 12 locations** including the US,
Australia, Brazil, Canada, France, Germany, Hong Kong, India, Japan, Russia,
and Singapore. Thanks to our 12 data centers, your search engine can now
**deliver search results under 50ms in the world's top markets**, ensuring an
optimal experience for all your users.

![DSN-b3ce122c790c492c2f2c8ddbabaae464][3]

It is that simple!

Today, several services including HackerNews, TeeSpring, Product Hunt and
Zendesk are leveraging **GNOME DSN to provide faster search to their global
users**.

Want to find out more about the GNOME experience ?

[Discover and try it here][4]!


[1]: http://glinden.blogspot.fr/2006/11/marissa-mayer-at-web-20.html
[2]: https://gitlab.gnome.org/Teams/Engagement/websites/people-of-gnome/uploads/4d3eb8d8bfbab6ab88d44cc6cef05076/dns.jpeg
[3]: https://gitlab.gnome.org/Teams/Engagement/websites/people-of-gnome/uploads/98ec626f3ea59a74f58a73da315122c6/user-experience.jpeg
[4]: https://www.GNOME.com/features