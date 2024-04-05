---
title: "Amber Carpio Take Home"
excerpt: "Vercel Take Home"
coverImage: "/assets/blog/dynamic-routing/cover.jpg"
date: "2024-04-05T05:35:07.322Z"
author:
  name: Amber Carpio
  picture: "assetss/blog/authors/amb.jpeg"
ogImage:
  url: "/assets/blog/dynamic-routing/cover.jpg"
---

## What do you want to learn or do more of at work?

What I love about Vercel is how it is developer focused. I would love to become an expert at app developement and work close with Engineering to better my skills. I love expanding my knowledge and putting what I learn to use.

## Describe how you solved a challenge or technical issue that you faced in a previous role (preferably in a previous support role). How did you determine that your solution was successful?

Working at Snyk, the challenge that I faced that sticks out the most is with a broker instance. I was able to overcome the challenge by using our intneral resources. This included searching past tickets for the same issue, searching slack messages, consulting Engineering, and using internal and external docs. You have to be thorough when facing a challenge and willing to research and think outside of the box.

## When would you choose to use Edge Functions, Serverless Functions, or Edge Middleware with Vercel?

Edge Functions: Opt for this cost effective choice when you need lightweight JavaScript functions that execute close to the user (https://vercel.com/docs/functions)

Serverless Functions: Gives you access to all the Node.js APIs that you would expect for writing on the web, with the ability to configure machine resources and dependencies (https://vercel.com/docs/functions)

Edge Middleware: Because it runs before the cache, using Middleware is an effective way of providing personalization to statically generated content. (https://vercel.com/docs/functions/edge-middleware)

## Imagine a customer writes in requesting help with a build issue on a framework or technology that you've not seen before. How would you begin troubleshooting this and what questions would you ask the customer to understand the situation better?

Hi there,

From my understanding you are using example framework. If you haven't seen our documentation about our supported frameworks, please feel free to check out https://vercel.com/docs/frameworks. If you could please answer the following questions, I'd be more than happy to further assist.

    1. When using the exampleframework what error are you running into?
    2. If you are using the CLI, could you please provide us with the debug?
    3. If you happen to have any screenshots this would help us identify the root cause.

## The customer from question 5 replies to your response with the below: “I’m so frustrated. I’ve been trying to make this work for hours and I just can’t figure it out. It must be a platform issue so just fix it for me instead of asking me questions.” Please write a follow-up reply to the customer.

Hi there,

I completely understand and I want to ensure you have the best experiance with Vercel. In order to do so, I'd like to make sure that nothing was missed before addressing this on our side. With that being said, the questions I previously asked would help identify where we need to start to get this resolved for you. We want to make sure we have a good understanding of the way you are using Vercel.

## A customer writes in to the Helpdesk asking "How do I do a redirect from the /blog path to https://example.com?" Please write a reply to the customer. Feel free to add any information about your decision making process after the reply.

Hello there,

We recommend using the framework-native solution for dynamic redirects. You can use the following code snippet to redirect from the /blog path.

Serverless
(example)

Edge Functions
(example)

For more information on redirects, you can view our documentation:
https://vercel.com/docs/edge-network/redirects#configuration.

I made this decison based on the available documentation from Vercel. I believe this relates to Canonicalization of multiple URLs.

## A customer is creating a site and would like their project not to be indexed by search engines. Please write a reply to the customer. Feel free to add any information about your decision making process after the reply.

Hello there,

Since a Preview Deployment creates a new version of your site under a different domain, a search engine would consider it as a new website when crawling it.

This can have a negative impact on the ranking of your main site since crawlers are able to detect when content is duplicated across multiple domains and lower the ranking of your site when measuring the content quality.

To prevent that, the X-Robots-Tag HTTP header is automatically set to noindex for all Preview Deployments so that search engines do not accidentally index the Preview URLs.

When a custom domain is assigned to a Git branch, this behavior is prevented. In that case, the X-Robots-Tag header is not set.

To learn more about the X-Robots-Tag, review this Google Search Reference. (https://developers.google.com/search/docs/crawling-indexing/robots-meta-tag#xrobotstag)

You can also check out this helpful article from Vercel that explains more https://vercel.com/guides/are-vercel-preview-deployment-indexed-by-search-engines.

I made this decision based on Vercels documenation.

## What do you think is one of the most common problems which customers ask Vercel for help with? How would you help customers to overcome common problems, short-term and long-term?

I think the most common problems might be general setup or incidents. I think it is important to monitor status at https://www.vercel-status.com/ and be aware of current problems in case something comes in. For short term and long term problems, the key is to be involved, research, and communicate effectivly.

## How could we improve or alter this familiarisation exercise?

I was a little lost on if the exercise was support to be a part of the application. I first chose a chat GPT template and realize that would not work for this exercise, but a blog post would be more effective. On one of the blog post templates, it had an error deploying so I had to select a differnt one.
