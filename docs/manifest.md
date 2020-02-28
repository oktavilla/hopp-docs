---
layout: default
title:  "Manifest"
nav_order: 1
---

# Platform manifest
{: .no_toc }

The purpose is to outline what we believe is the right solution to what our customers need and what we can sell. The initial intention is to use this as an internal document for shared understanding.

1. TOC
{:toc}

## Our raison d'être

As a platform we want to help bootstrap new digital products and make it possible for existing businesses to reinvent their online editorial offerings.

Our platform enables media to become digitally native with best in class technology, tried and tested UX and modern digital business practices at its core. Without them having to become tech companies themselves.

## Being a Platform

A platform is more than just a kit of tools. A platform comes with a clear idea of how those tools fit together and how they should be utilised. It’s just as much a service as it is a product. 
Features, patterns and know-how should (at least potentially) benefit everyone on the platform. For that reason the platform can not only enable but must also define, restrict and provide guidance. We don’t develop for individual clients, we develop for the platform. 
* The platform is opinionated.
* The platform is governed.

A platform must be built to scale. For something to be able to grow over time we must ensure a solid base. We need to be able to trust that core principles last over time and we need to be able to switch out isolated parts without critically affecting the system as a whole.
* The platform should be based on solid data models. 
* Data models should have distinct purposes in relation to others.
* The platform should consist of distinct parts where each component has a clear role that does not overlap with others.
* Platform parts integrate with each other using clearly defined contracts.

The platform must be built so that new clients can be onboarded easily at any time. It should mostly be a matter of configuration and setup.
The platform must be designed in such a way that improvements can be rolled out continuously without clients having to take specific measures or actively approve changes.
* New platform features must not break any design or functionality for existing clients. 
* Changes to existing information design or features should be handled TBD.

## Basic Concepts

In the platform we define an Editorial Product as a user experience and a selection of content targeted and packaged with a specific audience in mind. 

An Editorial Product serves content from a Content Pool. In most scenarios this is a 1/1 relationship, but additional Editorial Products can be set up to serve subsets of content from one pool. An Editorial Product can be a website, a newsletter or an app depending on how it is intended to best be accessed and consumed by its target audience. These different product types share a lot of things but they differ in some aspects. 

A set of Editorial Products and its Content Pool is referred to as LOREM IPSUM. This is usually, but not always, a brand. 

This is where the concept of an Editorial Team comes in play. We define an Editorial Team as the people and roles that work with a LOREM IPSUM. Organisational concepts such as departments or different professional roles does not exist in the platform.

An organisation with several LOREM IPSUMs may want to leverage content created in one Content Pool for use in others. For this purpose it is possible to set up a Content Network. See Content Sharing for more information on this. 

## Product Experience

What your users experience when interacting with your editorial product is multi faceted. It’s not just about how it looks. The way it feels is arguably even more important. The platform provides a set of “Product Experience Layers” that all work together to create a beautiful, useable and coherent user experience. The first Product Experience Layer ensure that your product is state of the art when it comes to readability, usability and accessibility. This is the baseline that your product deserve and what your readers expect. The second layer defines the overall structure and enables or disables specific functionality for your product. The third layer is what makes it truly yours. 

### Information Design Templates

The platform comes with a set of pre tested and pre optimised Information Design Templates. There are Articles, Start page, Tag pages, Authors and many more. These templates are part of the platform itself and forms the basis of what your users can see and do. Basically the templates define the order and hierarchy of everything that goes on a page. 

Bound with the templates the platform also comes with an out-of-the-box, best-practice Design Patterns System. This is a set of rules that define the basics for how products on the platform will look and behave. The rules describe – in visual terms – how all common components like columns, teasers, bylines, dividers and article lists should look and behave. On all and any screen size. This is the first layer.

### Product Configuration

A product can be tailored to specific needs with configuration options. The options differ depending on the type of product (website or editorial newsletter). For a website you may configure a start page mix, define navigation, tweak teasers, enable or disable ads positions etc. This is the second layer.

### Brand Identity

With the first layer (Information Design Templates) pre applied for all products on the platform you’re already guaranteed great readability, usability and device accessibility. But in order to charge the user experience with the trust and recognisability of your Brand the Information Design Templates comes with a set of “hooks”. With the Brand Identity Layer we apply your own specific typography, colors, backgrounds etc. 

## Editorial Content

One of the main areas where the platform differs from generic CMSes is how you work with content. 

Editorial content is generally dynamic by nature. You should always be able to tell stories the best way possible. Journalism is a creative process involving skills like pedagogy, psychology, empathy and knowledge. A journalist needs a story telling toolbox, not a form. So the standard article on the platform comes with a free form content editor where you can mix and match different types of content blocks and media. An article is very simple in its basic form. It consists of a title, a lead, a main image and a set of content blocks. 

Sometimes you want to tell stories through other means than text or mixed media. Therefore the platform also comes with dedicated content types like video and audio. The purpose for this is to provide information about the way the content is intended to be primarily consumed. 

## Content Promotion and Visibility

For your content to be found, read and loved you need to promote it in different ways. There’s all types of external promotion that you can do like social media posting, search engine advertising, cross posting etc. These activities are not supported per se on the platform. The platform does however make sure that you have all the tools you need to ensure content visibility in external platforms.

## Internal Promotion

Besides promoting your content in external channels it is paramount to make sure users are able to find relevant content when they’re interacting with your product. This is where internal promotion comes into play. Internal promotion happens on the start page, on editorial section pages, in recirculation blocka on articles or on tag, category, brand pages etc.

## Monetisation

### Premium Content

There’s a general paywall setting for each product. This setting is defined in the product configuration and can be set to “off”, “free” or “premium”. This determines the current default for the product. The general paywall setting can be overridden on specific articles by flagging them as “always premium” or “always free”. 

If the General Paywall setting is “on” customer access to content is negotiated case-by-case by a “broker service”. The broker determines if an article is to be considered “premium” based on the general paywall setting but takes any overrides on the current article into regard. If the content is determined to be “premium” the broker will check the access rights of the current user. For a user to get access to premium content they need to be logged in and flagged as “eligible to premium content”. 

If content is determined to be “premium” but the user is not eligible they will be presented with a call to action. This can either be to log in or to sign up/subscribe. These components can be defined somewhere.

Premium content is available for search engines at all times. For further information about access rights and customer management see Authentication and Customer Management respectively.

### Display Ads

There are a number of Display Ad placements and formats that can be used for third-party advertising solutions (i.e. 
Google Ad Manager). The platform comes with several pre defined placements in the header, on articles and on the start page. You can pick and choose which ones to use in the Editorial Product configuration.

### Native

Church and State. Separate simplified Content Pool. Fed into product. How to promote?

### Branded/partner content

Branded or sponsored content is produced in the same Content Pool as other editorial content. This can be any type of content as long as it is tagged with a partner. All content attributed to a partner will be clearly marked as such. 

Every partner will have its own page where they can be presented and have all sponsored content listed. A partner can also sponsor tags and sections. Any content with that tag or in that section will then be attributed to the partner.

## Customer Access and Management

TBD
