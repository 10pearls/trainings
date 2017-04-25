
# Self Learning Program:

## 1. Getting Started

### Introduction to Web API - Rest api concepts
ASP. NET Web API is a framework that makes it easy to build HTTP services that reach a broad range of clients, including browsers and mobile devices. ASP. NET Web API is an ideal platform for building RESTful applications on the .NET Framework. More about [Web API].

### Action Result in Web API
When you are developing an ASP. NET Web API application, you can choose whether you want to return an instance of HttpResponseMessage, IHttpActionResult or an Entity of any type from your action, which will then be serialized. There are four [Action Results] supported by  Web API.

### Http status Codes
HTTP response status codes indicate whether a specific HTTP request has been successfully completed. Responses are grouped in five classes: informational responses, successful responses, redirects, client errors, and servers errors. Read more details about [status codes].

### Http Request methods
HTTP defines a set of request methods to indicate the desired action to be performed for a given resource. Although they can also be nouns, these request methods are sometimes referred as HTTP verbs. Each of them implements a different semantic, but some common features are shared by a group of them: e.g. a request method can be safe, idempotent, or cacheable.
More details about [Http Request Methods].

## 2. Routing
Routing is how Web API matches a URI to an action. If you are familiar with ASP. NET MVC, Web API routing is very similar to MVC routing. The main difference is that Web API uses the HTTP method, not the URI path, to select the action.

Go to [Routing] to read more about it.

### Attribute Routing
 Web API 2 supports a new type of routing, called attribute routing. As the name implies, attribute routing uses attributes to define routes.
 
Read more about [Attribute Routing] here.

## 3. Working with data
Entity Framework (EF) is an object-relational mapper that enables .NET developers to work with relational data using domain-specific objects. It eliminates the need for most of the data-access code that developers usually need to write.

[Entity Framework Db first]

[Entity Framework Code first]

[Entity Framework Model first]

[More info on EF approaches]

### DTO
A DTO is an object that defines how the data will be sent over the network. Read more about [DTO]. 

## 4. Serialization and Model Binding

### JSON and XML Serialization in Web API
Web API provides media-type formatters for both JSON and XML. Go to [JSON and XML Serialization in ASP.NET Web API] for details.

### Media Formatters in Web API
A media type, also called a MIME type, identifies the format of a piece of data. In HTTP, media types describe the format of the message body. Read more about [Media Formatters].

### Model Validations and Annotations
When a client sends data to your web API, often you want to validate the data before doing any processing. This article shows how to annotate your models, use the annotations for data validation, and handle validation errors in your web API. Read more about [Model Validations and Annotations].

## 5. Error Handling

### Exception Handling
Error that occur at runtime are called as Exceptions. Exception handling should be done to handle such errors. You should have a good idea of how you can handle exceptions in Web API and send out appropriate error codes and error messages from your Web API controller methods.

There are several ways to handle exceptions.

[Http Response Handling]

[Http Error]

[Exception Filter]

### Logging

Logging could be very beneficial and helps us in a lot of ways such as debugging, tracing, monitoring and analytics. You can use different tools for logging or implement your own custom log module.

[Log4Net]

[Custom Logging]

## 6. Security
Security in itself is very complicated and tricky topic. When we plan to create an enterprise level application, we especially want to take care of authentication and authorization. These are two techniques if used well makes our application secure, in our case makes our WebAPI more secure.

### Authentication: 
Authentication is all about the identity of an end user. It’s about validating the identity of a user who is accessing our system, that he is authenticated enough to use our resources or not. Does that end user have valid credentials to log in our system? Credentials can be in the form of a user name and password. We’ll use Basic Authentication technique to understand how we can achieve authentication in WebAPI.

Basic authentication is a mechanism, where an end user gets authenticated through the service with the help of user name and password. An end user makes a request to the service for authentication with user name and password embedded in request header. Here are details about [Basic Authentication].

### Authorization: 
Authorization should be considered as a second step after authentication to achieve security. Authorization means what permissions the authenticated user has to access web resources. This could be achieved by setting roles and permissions for an end user who is authenticated. See [Authentication and Authorization].

### OAuth 2:
OAuth 2.0 is the industry-standard protocol for authorization. Have a look at [implementing OAuth in Web API].

### ASP. Net Identity
ASP. NET Identity is the latest membership and identity management framework provided by Microsoft, this membership system can be plugged to any ASP. NET framework such as Web API, MVC, Web Forms, etc. Read more details about [ASP.NET Identity].

### Action Filters
An action filter is an attribute. You can apply most action filters to either an individual controller action or an entire controller. [ActionFilters] are a great way to add extra functionality to your Web API service.

## 7. Async and Sync API

Async and performance are often a considered to go hand in hand because performance is bracketed with scaling. ASP. NET provides [async] actions starting with .NET 4.5.

## 8. Dependency Injection
In software engineering, dependency injection is a technique whereby one object supplies the dependencies of another object. A dependency is an object that can be used (a service). An injection is the passing of a dependency to a dependent object (a client) that would use it.

### Autofac

[Autofac] is an open-source dependency injection (DI) or inversion of control (IoC) container developed on Google Code. 

See details about [dependency injection] here.

The [Autofac Web API example] could be used as an example from Autofac documentation.

### Unity
Unity is a Microsoft Dependency Injection Framework or DI Container. It can be downloaded from Codeplex or using NuGet from inside of Visual Studio. Dependency injection injects the dependencies of a class at runtime. Read more about [Unity] here.

 [Http Response Handling]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/error-handling/exception-handling#httpresponserexception>

 [Http Error]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/error-handling/exception-handling#httperror>
 
[Exception Filter]: <https://www.codeproject.com/Articles/722349/Exception-Handling-in-ASP-NET-Web-API-Part> 

[Custom Logging]: <http://arcware.net/logging-web-api-requests/> 

[Log4Net]: <http://devthings.com.ua/implementing-logging-for-asp-net-web-api-with-log4net/>

[Basic Authentication]: <https://stevescodingblog.co.uk/basic-authentication-with-asp-net-webapi/>

[Authentication and Authorization]: <https://code.tutsplus.com/tutorials/securing-aspnet-web-api--cms-26012>

[OAuth2]: <https://oauth.net/2/>

[implementing OAuth in Web API]: <http://www.c-sharpcorner.com/UploadFile/736ca4/token-based-authentication-in-web-api-2/>

[ASP.NET Identity]: <http://bitoftech.net/2015/01/21/asp-net-identity-2-with-asp-net-web-api-2-accounts-management/>

[ActionFilters]: <https://damienbod.com/2014/01/04/web-api-2-using-actionfilterattribute-overrideactionfiltersattribute-and-ioc-injection/>

[async]: <https://www.codeproject.com/Tips/805923/Asynchronous-programming-in-Web-API-ASP-NET-MVC>

[dependency injection]: <https://www.codeproject.com/articles/615139/an-absolute-beginners-tutorial-on-dependency-inver>

[Autofac]: <https://autofac.org/>

[Autofac Web API example]: <http://docs.autofac.org/en/latest/integration/webapi.html>

[Web API]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/getting-started-with-aspnet-web-api/tutorial-your-first-web-api>

[Action Results]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/getting-started-with-aspnet-web-api/action-results>

[status codes]: <https://developer.mozilla.org/en-US/docs/Web/HTTP/Status>

[Http Request Methods]: <https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods>

[Routing]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/web-api-routing-and-actions/routing-in-aspnet-web-api>

[Attribute Routing]:  <https://docs.microsoft.com/en-us/aspnet/web-api/overview/web-api-routing-and-actions/attribute-routing-in-web-api-2>

[JSON and XML Serialization in ASP.NET Web API]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/formats-and-model-binding/>

[Media Formatters]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/formats-and-model-binding/media-formatters>

[Model Validations and Annotations]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/formats-and-model-binding/model-validation-in-aspnet-web-api>

[Entity Framework Code first]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/data/using-web-api-with-entity-framework/>

[Entity Framework Db first]: <http://www.tutorialsteacher.com/webapi/create-web-api-for-crud-operation>

[Entity Framework Model first]: <http://www.c-sharpcorner.com/UploadFile/4b0136/model-first-approach-in-Asp-Net-mvc-5/>

[More info on EF approaches]: <http://www.c-sharpcorner.com/UploadFile/ff2f08/identifying-entity-framework-development-approaches/>

[DTO]: <https://docs.microsoft.com/en-us/aspnet/web-api/overview/data/using-web-api-with-entity-framework/part-5>

[Unity]: <https://www.codeproject.com/Articles/988257/Dependency-Injection-using-Unity-container>