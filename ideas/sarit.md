# Sarit

An educational content curator to generate distraction-free educational feed of recommended content accross blog posts (through rss, atom etc), youtube videos etc.

## Why

Platforms like YouTube, Reddit are mostly _genre-agnostic_ feed generators that give the user a huge potential to fall into rabbit holes of meaningless content after deviating from the intended video/post.
Even though these platforms have immense potential to educate oneself on various topics in varying level of competence, most of this content does not reach the intended audience, as a large portion of the internet succumbs to the clickbait non-serious content due to these recommendation algorithms.
We need a platform that indexes, categorizes, (potentially tokenizes) and generate a productive feed of educational content that guarantees a distraction-free experience where every minute spent on the platform is something constructive or knowledgeable.

## How 

Sarit does not aim to do the heavy-lifting work of hosting, moderating and allowing the creation of content on the platform in general.
It is just a content curator.
Just like Hackernews is simply a platform to post cool tech stuff from accross the internet, Sarit is a platform that crawls, or accepts suggestions for new content.
It categorizes the new content and serves it in the recommendation feeds of it's users who would potentially be interested in the suggested content.

The sources of the content can be various platforms such as Youtube, Reddit, Atom/RSS feeds of popular blogs, journals, or simply cool explainer websites. There is no restriction in the format of the content apart from the will of the creator.
However, keep in mind that it must be able to index the content type that it accepts/crawls.

Efforts should be made to ensure that the suggested content to any user is relevant to his/her interests based on his/her history or preferences submitted during registration process.

## Challenges Faced

The biggest challenge is creating/using a recommendation model for curating the content.

The second biggest challenge is getting a metric to judge how much the user likes/dislikes the suggestion. A classic approach would be to implement upvote/downvote features, but other metrics of engagement might be challenging for content as it is not hosted by Sarit.

The third challenge is to explore the legalities of crawling and indexing third party content, which must be ensured before new content is being added to the platform.

## Good to have features

A comment system with minimalistic rewards for the content shown in the feed is a nice-to-have feature (just like Hackernews).

Although it is difficult to monetize a content curation platform, features like donations (think Patreon), for the users to help their favourite content creators would be very useful.

contributed by [Kush Patel](https://github.com/libkush)
