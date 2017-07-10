---
title: Debugging Google App Engine and Cloud Endpoints with IDE
date: 14:00 07/09/2017
author: Ahumaro Mendoza
taxonomy:
    category: blog
    tag: [cloud, backend]
---

#### Platform as a Service (PaaS) or the so called Serverless infrastructure

At the present time, when we talk about Cloud Computing the first scenarios we think about are Virtual Machines hosted somewhere in the cloud, managed by ourselves and with complete freedom to customize the O.S. and all the tools and frameworks a la carte. Other scenario are the so popular Containers, like Docker, where we can create microservices and can be managed with some kind of orchestration system like Kubernetes.

But, there is another scenario, IMHO, the most forgotten and less marketed of all: The so called Serverless, or, being strict, the **Platform as a Service (PaaS)** scenario. In this environment, you are not able to manage a virtual machine nor a container. You only focus all your effort in your applications and you can deploy your code into this infrastructure and the platform is in charge to run, scale, and protect your invention.

It’s marvelous because you only pay what you use, and you are free of the concernings of actualizations of the O.S., scaling and all that bad nightmares. 

All these goodies don't come at a free price of course. There are some restrictions you have to live with, like the languages supported and, in some cases, you cannot use the full set of the language selected (in the case of Java, for example, multithreading, sockets, etc.).

If you can live with those caveats, then, try it, you will be glad for the simplicity and effortless of putting some code in the cloud.

One of those infrastructures among others is **Google App Engine**. It’s very easy to use and really affordable. The best of all, your code runs on the same infrastructure Google use for some if its products. Also, many frameworks can run on top of it, for example, **Google Cloud Endpoints**: One of the best and easiest ways to build and publish an API that can be consumed by iOS, Android and Web clients. It can be a RESTful API, a gRPC based, Open API, among others.


>>>>>> For more information about **PaaS**, **GAE** and **GCE** use the following links:

>>>>>> [**Platform as a Service (PaaS)**](https://en.wikipedia.org/wiki/Platform_as_a_service)
>>>>>> **|** [**Google App Engine**](https://cloud.google.com/appengine)
>>>>>> **|** [**Google Cloud Endpoints**](https://cloud.google.com/endpoints/)

#### Using an IDE for coding and debugging

Using an **IDE** is not a rule when you are going to develop some code for Google App Engine. Google has developed the frameworks with an IDE agnostic way in mind so you can even use notepad or vi to develop your product.

You can use **Maven** or **Gradle** to perform some of the basic tasks in the build chain and also you can generate the required artifacts to deploy your next API in the cloud.

In the other hand, for some tasks, it’s easier to have a good IDE where you can have code completion, refactoring and all those sweeteners at developing time.

You can use any IDE you want, **Eclipse** is very common and widely spreaded. This time I will be using **IntelliJ** but the theory is the same for any IDE you want.

Under the hood we will be using Gradle tools to perform the build and deploy tasks but the IDE will help us at coding time and also to debug step by step the code that will be running via **Gradle** and using the remote debugger capability of the IDE.

>>>>>> **IMPORTANT**: For simplicity, there are some steps omitted. Only the strictly necessary steps to make the project run and debug in the IDE are depicted in this article.

>>>>>> Use this link to find out more information about developing an API using Google Cloud Endpoints and all the required steps and best practices: [**Google Cloud Endpoints Documentation**](https://cloud.google.com/endpoints/docs/)

#### Importing the project into IDE

For demonstration purposes, we will use one of the examples available in the Google’s Git repository: The **Google Cloud Endpoints backend** example.

>>>>>> In the following link you can get the full set of examples developed by Google to demonstrate some of the Google Cloud capabilities: [**java-docs-samples**](https://github.com/GoogleCloudPlatform/java-docs-samples)

>>>>>> We will be working with this particular example: [**App Engine Standard & Google Cloud Endpoints Frameworks & Java**](https://github.com/GoogleCloudPlatform/java-docs-samples/tree/master/appengine-java8/endpoints-v2-backend)

Checkout the code and store it somewhere in your computer. Then, open your IDE, in this case I will be using **IntelliJ**.


#### Initialize the code to first compile/build.

#### Directives to make the code debuggable.

#### Remote debug on the IDE


### Keep exploring and enjoy!

**Ahumaro Mendoza**<br/>
ahumaro@ahumaro.com<br/>
www.ahumaro.com
