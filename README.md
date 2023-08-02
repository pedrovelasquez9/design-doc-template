# Programación en español's blog with Astro

## Authors

- [Pedro Plasencia](https://github.com/pedrovelasquez9)

## Overview

This would be a blog for "Programación en español" community, the idea is to have documental technical content with a "retro" design and focused on the static content and web performance.

The goal of the project is to board the technical content from a documental perspective for the community members that prefer blog articles instead of video/audio formats.

## Context

The goal of this initiative is to have a documental/blog post format for those users in the community that prefers to read tutorials, tips and programming subjects instead of video/audio only content inside "Programación en español".

## Goals

- Centralize posts about technologies and learning for hispanic programming community
- Have an standalone ad-hoc solution for a blog destinated for "Programación en español" community and it's creator

## Non-goals

- This will not be a full Wordpress-like CMS, the blog will be static and markdown based for the posts
- This will not be a blog based on subscriptions and, at least in early versions, will not have a newsletter or user information handling in any case
- We can identify, at least, two types of users (authors and readers), nevertheless, we'll not have any credential system, as the authors will have to make a PR to the project's repository to upload new posts.
- The blog will not gather any visitor's information whatsoever for metrics or any other purpose

## Proposed solution

- As a general solution, we'll have a blog with two types of users (end user or reader and authors)
- If there's a new post author in the blog, the person should make a repository fork and a pull request with new posts under a specific category

### Author use case

- insert flow chart here

### Reader use case

- insert flow chart here

## Alternative solutions

### Wordpress custom installation

- Pros:
  - Easy to install and manage based on credentials
  - More measured information about visits and statistics
  - More options and integrations for newsletter, ads, etc.
- Cons:
  - Doesn't fit the required "retro" style
  - Does not point to static content, so it could have performance issues
  - Gathers not necessary user information

## Monitoring

- We could use an open source service for visit and site health monitoring that doesn't require user's data

## Cross-team impact

- The main impact it'll have is the automatic deployment process (devops), the test and the secret credential configuration for this pipeline and deployment flow
- This could have some vulnerability risks if the server's credentials are exposed or not well handled with github secrets store

## Scoping and timeline

- Create base project with Astro
- Define and create categories
- Create route system based on categories
- Create and show posts in .md format inside those categories
- Apply retro style
- Check and apply responsive design
- Improve web performance
- Configure automated deployment
- Test deployment
- Configure sub-domain
- Point sub-domain to deployed project
- Test redirection and web rendering and routing
