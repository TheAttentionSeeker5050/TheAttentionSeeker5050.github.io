---
layout: project-item
title: "Ad Board with Spring Boot and Angular"
backendRepository: https://github.com/TheAttentionSeeker5050/ad-board-with-java-spring-boot
frontendRepository: https://github.com/TheAttentionSeeker5050/kaijoo-ad-board-frontend-web-angular
---

<p id="heading-p">
    Kaijoo is an ad board where users can post or browse among different classified ads categories. Made on the following technologies: Spring Boot, JBDC and MySQL (backend) and Angular(frontend)
</p>

## Features
- User can create an account
- User can login
- User can create a post
- User and anonymous user can view all posts
- User and anonymous user can view a single post
- User can update a post
- User can delete a post
- Advanced search option with semantic search capabilities
- Admin user can add or modify tags, categories, subcategories
- Post can have multiple media items and social media links
- This API will be integrated with a messaging service such as firebase to allow users to communicate with each other.
- This API will be integrated with a front end application that will consume the API.

## Data Models
- Post: Each individual post that users can create.
- Category: Categories of post
- Tag: Tags associated to posts
- User: The users, they can either be admin or regular users, they can buy or sell goods and services.
- MediaItem: A media item url associated to a post, these can be videos, images, recordings, etc.
- SubCategory: SubCategories of posts
- SocialLink: Social links associated to a post
- Convesation: This hold the id of the conversations as well as the id of the users that are part of the conversation. This will play a role when integrating to a messaging service such as firebase.

## Angular Components
- Main app, holds everything, can have header, footer or not
- Login and Register: Dont have header and footer
- Home screen like any other site of this kind, has options, browse by category/subcategory, by tag
- User profile screen, has dashboard and options
- Post listing and Post list screen
- The editor screen for categories and subcategories, only accessible for admin users