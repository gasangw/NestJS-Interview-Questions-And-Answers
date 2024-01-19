# NestJS Interview Questions & Answers

> Welcome to the NestJS Interview Questions and Answers repository! 
- This repository aims to be a comprehensive resource for NestJS developers preparing for interviews. Whether you're a beginner or an experienced developer, this collection of questions and answers is designed to help you brush up on your NestJS knowledge and excel in interviews.
> Click ⭐if you like the project and incase you're interested in contributing to this project. Before you dive in, please take a moment to review our guidelines.

## Important Links

- [Code of Conduct](./CODE_OF_CONDUCT.md): We expect everyone participating in this project to follow our code of conduct. Make sure you understand and adhere to these guidelines.

- [Contributing Guidelines](./CONTRIBUTING.md): Before contributing, please read our contributing guidelines. They provide information on how to submit questions, report issues, and more.

> Follow me [@gasangw](https://github.com/gasangw).

### Table of Contents

| No. | Questions                                                                                                                                                         |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [What is Nestjs](#what-is-nestjs)     
| 2   | [Who developed NestJS? Why did they develop NestJS?](#Who-developed-NestJS?-Why-did-they-develop-NestJS?)   
| 3   | [When was NestJS first released?](#When-was-NestJS-first-released?)    
| 4   | [How can you install NestJS and set up a new project on your machine?](#How-can-you-install-NestJS-and-set-up-a-new-project-on-your-machine?)                                  |
| 5   | [What’s the difference between NestJS and Angular?](#What’s-the-difference-between-NestJS-and-Angular?)                                  |
| 6   | [Is it possible to use other languages like C++, Ruby or Python with NestJS? If yes, then how?](#Is-it-possible-to-use-other-languages-like-C++,-Ruby-or-Python-with-NestJS?-If-yes,-then-how?)
| 7   | [What are the main components of a NestJS application?](#What-are-the-main-components-of-a-NestJS-application?) 
| 8   | [How to declare a class as a controller in Nest.js](#How-to-declare-a-class-as-a-controller-in-Nest.js)     
| 9   | [Can you explain how to use decorators in a NestJS controller?](#Can-you-explain-how-to-use-decorators-in-a-NestJS-controller?) 
| 10   | [How can you use route parameters in a NestJS controller?](#How-can-you-use-route-parameters-in-a-NestJS-controller?) 
| 11   | [What is the role of the `@Body()` decorator?](#What-is-the-role-of-the-`@Body()`-decorator?) 
| 12   | [What is an interceptor in the context of NestJS?](#What-is-an-interceptor-in-the-context-of-NestJS?) 
| 13   | [What are pipes in the context of NestJS?](#What-are-pipes-in-the-context-of-NestJS?) 


### Answers


1. ### What is Nestjs

   Nest(NestJS) is a framework for building efficient, scalable Node.js server side applications. It uses progressive JavaScript and its built with and fully suports Typescript.

2. ### Who developed NestJS? Why did they develop NestJS?
    
    NestJS was developed by Kamil Myśliwiec, who is a Polish software engineer. He developed NestJS to address the lack of a consistent structure in Node.js applications and to bring powerful features of frameworks like Angular to the server-side.

3. ### When was NestJS first released?
    NestJS was first released on October 5, 2016.

4. ### How can you install NestJS and set up a new project on your machine?
    To install NestJS on your machine, you need to have Node.js and npm (Node Package Manager) installed. Once you have those, you can install the NestJS CLI (Command Line Interface) globally on your machine using the following command:
    ```javascript
      $ npm i -g @nestjs/cli   
    ```
    This command installs the `NestJS CLI` globally, which allows you to use the nest command from anywhere on your machine. With the NestJS CLI, you can create new projects using 
    ```javascript
      $ nest new project-name
    ``` 
    and after creating a project you can generate NestJS modules, services, etc.
    ```javascript
     $ nest generate module users
    ```
    running
    ```javascript 
      $ nest g resource users
    ```
    will several files that work together to handle CRUD (Create, Read, Update, Delete) operations for a particular entity, in this case, "users". It will generate:
    A `controller` for handling HTTP requests (e.g., users.controller.ts)
    A `service` for business logic (e.g., users.service.ts)
    A `module` to encapsulate the resource (e.g., users.module.ts)
    If you choose to generate a REST API, it will also generate `DTO` (Data Transfer Object) classes for handling input data (e.g., `create-user.dto.ts, update-user.dto.ts`)
    If you choose to generate a GraphQL API, it will also generate a resolver (e.g., `users.resolver.ts`)

5. ### What’s the difference between NestJS and Angular?
    Angular is a framework for building client-side applications and It provides a way to organize your frontend code using components, modules, services, etc. while NestJS is a framework for building server-side applications. NestJS is built on top of TypeScript and Express, and it aims to provide a more robust and scalable architecture for enterprise-level applications. However It's heavily inspired by Angular and shares similar concepts like modules, decorators, and dependency injection.

6. ### Is it possible to use other languages like C++, Ruby or Python with NestJS? If yes, then how?
    Yes, it is possible to use other languages with NestJS. NestJS is language agnostic, meaning that it can work with any language that can compile to JavaScript.
    As for Python, Ruby, or other languages, they can't be used directly with NestJS because NestJS relies on the Node.js runtime, which executes JavaScript. As for Python, Ruby, or other languages, they can't be used directly with NestJS because NestJS relies on the Node.js runtime, which executes JavaScript. However, you can certainly build separate services in Python, Ruby, or any other language, and have them communicate with your NestJS application via HTTP, gRPC, or any other communication protocol. This is a common pattern in microservices architecture.

7. ### What are the main components of a NestJS application?
    The main contents of the nestjs application inlcude: 
    `Modules:` Modules are a way of organizing related components into a single block. They provide a way to structure your application.
    `Controllers:` Controllers are responsible for handling incoming `requests` and returning `responses` to the client.Controllers organize routes and handle HTTP requests that come to those routes.
    `Services:` services are responsible for business logic and interacting with data sources. They can be injected into controllers or other services, promoting code reusability and separation of concerns.

8. ### How to declare a class as a controller in Nest.js

    In Nest.js we can declare a class as a controller by using the **@Controller()** decorator. Here is a basic example.

    ```javascript
      import { Controller, Get } from '@nestjs/common';
      
      @Controller('example')
      class ExampleController {

         @Get()
         getHello(): string {
            return 'Hello world!';
         }
     }
    ```
    In this example the `ExampleController` is a controller class. **@Controller('example')** decorator tells Nest.js that this class is a controller that should handle requests to the `example` route. The **@Get()** decorator on the `getHello` method indicates that this method should handle HTTP GET requests.

    **[⬆ Back to Top](#table-of-contents)**

 
9.  ### Can you explain how to use decorators in a NestJS controller?
    Decorators in a NestJS controller are used to define routes and to handle different types of HTTP requests. For example, `@Get()`, `@Post()`, `@Put()`, `@Delete()` are used to handle GET, POST, PUT, DELETE requests respectively.
    ```javascript
    import { Controller, Get, Param, Body, Post, Patch, Delete } from '@nestjs/common';

    @Controller('cats')
    export class CatsController {
      @Get()
      findAll(): string {
        return 'This action returns all cats';
      }

      @Get(':id')
      findOne(@Param('id') id: number): string {
        return `This action returns a cat with the provided id`;
      }

      @Post()
      create(@Body() body: any): string {
        return `This action returns the body of the cat`;
      }

      @Patch('id')
      update(@Param('id') id: number, @Body() body: any ): string {
        return `This action updates the body of the cat`;
      }

      @Delete('id')
      remove(@Param('id') id: number): string {
        return `This action removes a cat`;
      }
    }

    ```
    **[⬆ Back to Top](#table-of-contents)**
  
10. ### How can you use route parameters in a NestJS controller?
    Route parameters in a NestJS controller can be accessed using the `@Param()` decorator in the controller methods.
    ```javascript
        @Patch('id')
        update(@Param('id') id: number, @Body() body: any ): string {
           return `This action updates the body of the cat`;
        }
    ```
    **[⬆ Back to Top](#table-of-contents)**

11. ### What is the role of the `@Body()` decorator?
    The `@Body()` decorator in NestJS is used to extract the entire body of the incoming HTTP request. It's commonly used in methods that handle POST and PUT requests where data is sent in the body of the request.

    For example, if you have a method in your controller to create a new user, you might use the `@Body()` decorator to get the user data from the request:
    ```javascript
     @Post()
     create(@Body() createUserDto: CreateUserDto) {
      return this.usersService.create(createUserDto);
     }
    ```
    In this example, createUserDto is an object that contains the data sent in the request body. The @Body() decorator automatically parses the JSON request body and assigns it to the createUserDto parameter.
    
    **[⬆ Back to Top](#table-of-contents)**

12. ### What is an interceptor in the context of NestJS?
    An interceptor is a class annotated with the `@Injectable()` decorator and implements the `NestInterceptor interface`.
    An Interceptor is function that can be used to intercept incoming requests to a NestJS application and perform some sort of manipulation before the request is handled by the route handler. This can be useful for things like logging, authentication and so on.
    An Interceptor has a set of useful capabilities which are inspired by the `Aspect Oriented Programming (AOP) technique` Aspect Oriented Programming is a `programming paradigm` that aims to increase `modularity` by allowing the separation of cross-cutting concern. 
    Interceptors make it possible to:
    `Binding extra logic before / after method execution:` An Interceptor can execute logic before and after a method is executed. This can be useful for tasks like logging, transforming the result of a method, or handling errors.
    `Transforming the result returned from a function:` An Interceptor can transform the response returned from a method. For example, you could use an interceptor to transform all responses to have a specific format.
    `Handling errors:` An Interceptor can also handle errors thrown within your application. This can be useful for logging or transforming errors before they're sent to the client.
    Here is an example of an interceptor that logs the user interactions as shown in the [Nestjs document](https://docs.nestjs.com/interceptors)
    ```javascript
      import { Injectable, NestInterceptor, ExecutionContext, CallHandler } from '@nestjs/common';
      import { Observable } from 'rxjs';
      import { tap } from 'rxjs/operators';

      @Injectable()
      export class LoggingInterceptor implements NestInterceptor {
        intercept(context: ExecutionContext, next: CallHandler): Observable<any> {
          console.log('Before...');

          const now = Date.now();
          return next
            .handle()
            .pipe(
              tap(() => console.log(`After... ${Date.now() - now}ms`)),
            );
        }
      }
    ```
    **[⬆ Back to Top](#table-of-contents)**

13. ###  What are pipes in the context of NestJS?
    Pipes are a feature of NestJS that allows for validation or transformation of data before it is passed to a route handler and can either return the arguments as is, modify them, or throw an exception.
    A pipe is a class annotated with the `@Injectable()` decorator, which implements the `PipeTransform interface`
    `Validation:` This is the most common use case for pipes. They can be used to validate incoming data to ensure it matches a certain data schema. If the data is invalid, the pipe can throw an exception to prevent the route handler from being executed.

    **[⬆ Back to Top](#table-of-contents)**
    