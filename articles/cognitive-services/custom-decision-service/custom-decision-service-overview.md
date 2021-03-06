---
title: What is Custom Decision Service? - Azure Cognitive Services | Microsoft Docs
description: This article overviews Azure Custom Decision Service, a cloud-based API for contextual decision-making that sharpens with experience.
services: cognitive-services
author: alekh
manager: slivkins
ms.service: cognitive-services
ms.topic: article
ms.date: 05/08/2018
ms.author: slivkins;marcozo;alekh;marossi
---
# What is Custom Decision Service?

Azure Custom Decision Service helps you create intelligent systems with a cloud-based, contextual decision-making API that sharpens with experience. Custom Decision Service uses reinforcement learning and adapts the content in your application to maximize user engagement. The system includes user feedback into its decisions in real time and responds to emergent trends and breaking stories in minutes.

In a typical application, a front page links to several articles or other types of content. As the front page loads, it requests the Custom Decision Service to rank articles included on the page. When you choose an article, a second request is sent to the Custom Decision Service that logs the outcome of that decision.

Custom Decision Service is easy to use. The easiest integration mode requires only an RSS feed for your content and a few lines of JavaScript to be added into your application.

Custom Decision Service converts your content into features for machine learning. The system uses these features to understand your content in terms of its text, images, videos, and overall sentiment. It uses several other [Microsoft Cognitive Services](https://www.microsoft.com/cognitive-services), like
[Entity Linking](../entitylinking/home.md),
[Text Analytics](../text-analytics/overview.md),
[Emotion](../emotion/home.md), and
[Computer Vision](../computer-vision/home.md).

Some common-use cases for Custom Decision Service include:

* Personalizing articles on a news website
* Personalizing video content on a media portal
* Optimizing ad placements or web pages that the ad directs to
* Ranking recommended items on a shopping website.

Custom Decision Service is currently in *free public preview*. It can personalize a list of articles on a website or an app. The feature extraction works best for English language content. [Limited functionality](../text-analytics/overview.md) is offered for other languages, like Spanish, French, German, Portuguese, and Japanese. This documentation will be revised as new functionality becomes available.

Custom Decision Service can be used in applications that are not in the content personalization domain. These applications might be a good fit for a custom preview. [Contact us](https://azure.microsoft.com/overview/sales-number/) to learn more.

## API usage modes

Custom Decision Service can be applied to both webpages and apps. The APIs can be called from either a browser or an app. The API usage is similar on both modes, but some of the details are different.

## Glossary of terms

Several terms frequently occur in this documentation:

* **Action set**: The set of content items for Custom Decision Service to rank. This set can be specified as an *RSS* or *Atom* endpoint.
* **Ranking**: Each request to Custom Decision Service specifies one or more action sets. The system responds by picking all the content options from these sets and returns them in ranked order.
* **Callback function**: This function, which you specify, renders the content in your UI. The content is ordered by the rank ordering returned by Custom Decision Service.
* **Reward**: A measure of how the user responded to the rendered content. Custom Decision Service measures user response by using clicks. The clicks are reported to the system by using custom code inserted in your application.

## Next steps

* [Register your application](custom-decision-service-get-started-register.md) with Custom Decision Service
* Get started to optimize [a webpage](custom-decision-service-get-started-browser.md) or [a smartphone app](custom-decision-service-get-started-app.md).
* Consult the [API reference](custom-decision-service-api-reference.md) to learn more about the provided functionality.