# Udagram Image Filtering Microservice

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

The project is split into three parts:
1. [The Simple Frontend](https://github.com/udacity/cloud-developer/tree/master/course-02/exercises/udacity-c2-frontend)
A basic Ionic client web application which consumes the RestAPI Backend. [Covered in the course]
2. [The RestAPI Backend](https://github.com/udacity/cloud-developer/tree/master/course-02/exercises/udacity-c2-restapi), a Node-Express server which can be deployed to a cloud service. [Covered in the course]
3. [The Image Filtering Microservice](https://github.com/udacity/cloud-developer/tree/master/course-02/project/image-filter-starter-code), the final project for the course. It is a Node-Express application which runs a simple script to process images. [Your assignment]

## Tasks

### Setup Node Environment

You'll need to create a new node server. Open a new terminal within the project directory and run:

1. Initialize a new project: `npm i`
2. run the development server with `npm run dev`

### Create a new endpoint in the server.ts file

The starter code has a task for you to complete an endpoint in `./src/server.ts` which uses query parameter to download an image from a public URL, filter the image, and return the result.

We've included a few helper functions to handle some of these concepts and we're importing it for you at the top of the `./src/server.ts`  file.

```typescript
import {filterImageFromURL, deleteLocalFiles} from './util/util';
```

### Deployed system

Elastic beanstalk endpoint: http://image-filter-tasd-dev.us-east-1.elasticbeanstalk.com/


### API testing
1) http://image-filter-tasd-dev.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://media.istockphoto.com/photos/giraffe-family-picture-id453469507?b=1%26k=20%26m=453469507%26s=170667a%26w=0%26h=pol4ebEcrSd-dnjsh8Z0_MhpG00ACyK5rVNo31ZyUe0=
2) http://image-filter-tasd-dev.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://media.istockphoto.com/photos/crossing-the-road-picture-id1200246941?b=1&k=20&m=1200246941&s=170667a&w=0&h=xGX2JDeZASqylTbOHmcx44p6eZ7JiNyNrE_DJiWfbZ0=

### Deployment screenshots
1) ![Alt text](/deployment_screenshots/to/elastic beanstalk deployment proof.png?raw=true "Title")
