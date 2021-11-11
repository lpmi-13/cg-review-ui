# Chaotic Good Review UI

This will be the frontend for the 3-tier application in the Chaotic Good project. It will show reviews as well as allow creating new ones and searching the current reviews.

## Features - User jouneys

The users will be able to navigate around in the UI to interact with reviews. They will be able to see information about a specific review as well as multiple reviews. They will also be able to submit a review and search across reviews by date/rating/keyword.

## Architecture

This is a simple react app with one main screen and search bar.

## Deployment

The static assets will be stored in S3 and used to populate a cloudfront distribution for the Chaotic Good project. This distribution will be created and deployed via the terraform stack in the main project.

This will be built via github actions and pushed to S3, so the only secrets we need are for an IAM role that is allowed to push to S3.
