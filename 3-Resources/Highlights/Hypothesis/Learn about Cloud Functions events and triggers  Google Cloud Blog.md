# Learn about Cloud Functions events and triggers | Google Cloud Blog

## Metadata

* Author: [cloud.google.com]()
* Title: Learn about Cloud Functions events and triggers | Google Cloud Blog
* Reference: https://cloud.google.com/blog/products/serverless/learn-about-cloud-functions-events-and-triggers
* Category: #Type/Highlight/Article

## Highlights

* Events are all kinds of activities or things like changes to data in a database, files added to a storage system, or a new virtual machine instance being created etc., that happen within a cloud environment that might require reactive action. Cloud Functions supports events from the following providers:HTTPCloud StorageCloud Pub/SubCloud FirestoreFirebase (Realtime Database, Cloud Storage, Analytics, Auth)Cloud Logging — [Updated on 2021-11-25 20:18:29](https://hyp.is/w2OBdE5WEeySeEsPSCPecQ/cloud.google.com/blog/products/serverless/learn-about-cloud-functions-events-and-triggers)  — Group: #Topic/Dev

* HTTP functionsHTTP functions can be invoked from standard HTTP requests. Clients sending these HTTP requests wait for the response synchronously, and HTTP functions can support handling of common HTTP request methods like GET, PUT, POST, DELETE, and OPTIONS.  — [Updated on 2021-11-25 20:18:34](https://hyp.is/xmWIVE5WEeyaQhdhkvnWYA/cloud.google.com/blog/products/serverless/learn-about-cloud-functions-events-and-triggers)  — Group: #Topic/Dev

* Event-driven functionsCloud Functions can use event-driven functions to handle events from your Cloud infrastructure, such as messages on a Pub/Sub topic, or changes in a Cloud Storage bucket. Cloud Functions supports two sub-types of event-driven functions:Background functions: Event-driven functions written for the Node.js, Python, Go, and Java Cloud Functions runtimes are known as background functions. See Writing Background Functions for more details.CloudEvent functions:  Event-driven functions written for the .NET, Ruby, and PHP runtimes are known as CloudEvent functions. See Writing CloudEvent Functions for more details. — [Updated on 2021-11-25 20:18:39](https://hyp.is/yUbVoE5WEeyP2JOBQIcLNA/cloud.google.com/blog/products/serverless/learn-about-cloud-functions-events-and-triggers)  — Group: #Topic/Dev

* Understanding event-driven architecture (EDA)Event-driven architecture (EDA) is a software architecture paradigm promoting the production, detection, consumption of, and reaction to events. This architectural pattern can be best applied to design and implement applications and systems that transmit events among loosely coupled software components and services. Putting everything together with an exampleThis example focuses on creating an event-driven architecture to build a service that analyzes RSS feeds content using managed services like Cloud Functions (event-driven), Cloud Scheduler, and the Google Cloud Machine Learning APIs. — [Updated on 2021-11-25 20:18:45](https://hyp.is/zUDp6E5WEeyPzvfR2c3crw/cloud.google.com/blog/products/serverless/learn-about-cloud-functions-events-and-triggers)  — Group: #Topic/Dev

* The above architecture illustrates the workflow of how an RSS feed can be analyzed as soon as it is collected. Here is the logic: Step 1: One RSS feed link will contain one or many URLs. Write a function to parse these URLs from RSS feed links and store them in a queue. Step 2: Write a function that reads URLs from the queue in Step 1, one by one, and download their web page contents. Store all web page contents in persistent storage.Step 3: Finally, write another function that reads web page contents from stored persistent storage in Step 2, analyze them, and write the results to another persistent storage target.  — [Updated on 2021-11-25 20:18:54](https://hyp.is/0mDHXk5WEeyTSAtylvPD3A/cloud.google.com/blog/products/serverless/learn-about-cloud-functions-events-and-triggers)  — Group: #Topic/Dev
