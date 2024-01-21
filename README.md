# NestJS Interview Questions & Answers

> Welcome to the NestJS Interview Questions and Answers repository!

- This repository aims to be a comprehensive resource for NestJS developers preparing for interviews. Whether you're a beginner or an experienced developer, this collection of questions and answers is designed to help you brush up on your NestJS knowledge and excel in interviews.
  > Click ⭐if you like the project and incase you're interested in contributing to this project. Before you dive in, please take a moment to review our guidelines.

## Important Links

- [Code of Conduct](./CODE_OF_CONDUCT.md): We expect everyone participating in this project to follow our code of conduct. Make sure you understand and adhere to these guidelines.

- [Contributing Guidelines](./CONTRIBUTING.md): Before contributing, please read our contributing guidelines. They provide information on how to submit questions, report issues, and more.

> Follow me [@gasangw](https://github.com/gasangw).

### Table of Contents

| No. | Questions                                                                                                                                                                                                                                       |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | [What is Nestjs?](#what-is-nestjs?)                                                                                                                                                                                                             |
| 2   | [Who developed NestJS? Why did they develop NestJS?](#who-developed-nestjs-why-did-they-develop-nestjs)                                                                                                                                         |
| 3   | [When was NestJS first released?](#when-was-nestjs-first-released)                                                                                                                                                                              |
| 4   | [How can you install NestJS and set up a new project on your machine?](#how-can-you-install-nestjs-and-set-up-a-new-project-on-your-machine)                                                                                                    |
| 5   | [What’s the difference between NestJS and Angular?](#what-s-the-difference-between-nestjs-and-angular?)                                                                                                                                         |
| 6   | [Is it possible to use other languages like C++, Ruby or Python with NestJS? If yes, then how?](#is-it-possible-to-use-other-languages-like-c-ruby-or-python-with-nestjs-if-yes-then-how)                                                       |
| 7   | [What are the main components of a NestJS application?](#what-are-the-main-components-of-a-nestjs-application)                                                                                                                                  |
| 8   | [How to declare a class as a controller in Nest.js](#how-to-declare-a-class-as-a-controller-in-nestjs)                                                                                                                                          |
| 9   | [Can you explain how to use decorators in a NestJS controller?](#can-you-explain-how-to-use-decorators-in-a-nestjs-controller)                                                                                                                  |
| 10  | [How can you use route parameters in a NestJS controller?](#how-can-you-use-route-parameters-in-a-nestjs-controller)                                                                                                                            |
| 11  | [What is the role of the `@Body()` decorator?](#what-is-the-role-of-the-body-decorator)                                                                                                                                                         |
| 12  | [What is an interceptor in the context of NestJS?](#what-is-an-interceptor-in-the-context-of-nestjs)                                                                                                                                            |
| 13  | [What are pipes in the context of NestJS?](#what-are-pipes-in-the-context-of-nestjs)                                                                                                                                                            |
| 14  | [What are guards in the context of NestJS?](#what-are-guards-in-the-context-of-nestjs)                                                                                                                                                          |
| 15  | [What are middlewares in the context of NestJS?](#what-are-middlewares-in-the-context-of-nestjs)                                                                                                                                                |
| 16  | [Explain the concept of Dependency Injection in NestJS. How does it help in building modular and testable applications?](#explain-the-concept-of-dependency-injection-in-nestjs-how-does-it-help-in-building-modular-and-testable-applications) |
| 17  | [What’s the difference between @injectable() and @inject() decorators?](#what-s-the-difference-between-injectable-and-inject-decorators)                                                                                                        |
| 18  | [How does the Nest logger differ from the standard console.log() and when would you prefer one over the other?](#how-does-the-nest-logger-differ-from-the-standard-console-log-and-when-would-you-prefer-one-over-the-other)                    |
| 19  | [What is the difference between interceptors and middleware?](#what-is-the-difference-between-interceptors-and-middleware)                                                                                                                      |
| 20  | [What testing frameworks work best with NestJS?](#what-testing-frameworks-work-best-with-nestjs)                                                                                                                                                |
| 21  | [Explain the purpose of DTOs (Data Transfer Objects) in NestJS.](#explain-the-purpose-of-dtos-data-transfer-objects-in-nestjs.)                                                                                                                 |
| 22  | [How can you handle asynchronous operations in NestJS, and what is the role of the Promise object?](#how-can-you-handle-asynchronous-operations-in-nestjs-and-what-is-the-role-of-the-promise-object)                                           |
| 23  | [Explain the purpose of the @InjectRepository() decorator in NestJS.](#explain-the-purpose-of-the-injectrepository-decorator-in-nestjs)                                                                                                     |
| 24  | [Explain the purpose of the @nestjs/jwt package in NestJS?](#explain-the-purpose-of-the-nestjs-jwt-package-in-nestjs)                                                                                                         |
| 25  | [Discuss how tokens are used for authorization in an API. What is the difference between authentication and authorization, and how are these processes implemented with tokens?](#discuss-how-tokens-are-used-for-authorization-in-an-api-what-is-the-difference-between-authentication-and-authorization-and-how-are-these-processes-implemented-with-tokens)                                                                                                         |
| 26  | [Why is it important for tokens to have an expiration time? How can you implement token expiration in NestJS, and what role do refresh tokens play in maintaining user sessions?](#why-is-it-important-for-tokens-to-have-an-expiration-time-How-can-you-implement-token-expiration-in-nestjs-and-what-role-do-refresh-tokens-play-in-maintaining-user-sessions)                                                                                                         |



### Answers

1. ### What is Nestjs?

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

   Angular is a framework for building client-side applications and It provides a way to organize your frontend code using components, modules, services, etc.

   while NestJS is a framework for building server-side applications. NestJS is built on top of TypeScript and Express, and it aims to provide a more robust and scalable architecture for enterprise-level applications. However It's heavily inspired by Angular and shares similar concepts like modules, decorators, and dependency injection.

6. ### Is it possible to use other languages like C++, Ruby or Python with NestJS? If yes, then how?

   Yes, it is possible to use other languages with NestJS. NestJS is language agnostic, meaning that it can work with any language that can compile to JavaScript.

   As for Python, Ruby, or other languages, they can't be used directly with NestJS because NestJS relies on the Node.js runtime, which executes JavaScript. As for Python, Ruby, or other languages, they can't be used directly with NestJS because NestJS relies on the Node.js runtime, which executes JavaScript.

   However, you can certainly build separate services in Python, Ruby, or any other language, and have them communicate with your NestJS application via HTTP, gRPC, or any other communication protocol. This is a common pattern in microservices architecture.

7. ### What are the main components of a NestJS application?

   The main contents of the nestjs application inlcude:
   `Modules:` Modules are a way of organizing related components into a single block. They provide a way to structure your application.

   `Controllers:` Controllers are responsible for handling incoming `requests` and returning `responses` to the client.Controllers organize routes and handle HTTP requests that come to those routes.

   `Services:` services are responsible for business logic and interacting with data sources. They can be injected into controllers or other services, promoting code reusability and separation of concerns.

8. ### How to declare a class as a controller in Nest.js

   In Nest.js we can declare a class as a controller by using the **@Controller()** decorator. Here is a basic example.

   ```javascript
   import { Controller, Get } from "@nestjs/common";

   @Controller("example")
   class ExampleController {
     @Get()
     getHello(): string {
       return "Hello world!";
     }
   }
   ```

   In this example the `ExampleController` is a controller class. **@Controller('example')** decorator tells Nest.js that this class is a controller that should handle requests to the `example` route. The **@Get()** decorator on the `getHello` method indicates that this method should handle HTTP GET requests.

   **[⬆ Back to Top](#table-of-contents)**

9. ### Can you explain how to use decorators in a NestJS controller?

   Decorators in a NestJS controller are used to define routes and to handle different types of HTTP requests. For example, `@Get()`, `@Post()`, `@Put()`, `@Delete()` are used to handle GET, POST, PUT, DELETE requests respectively.

   ```javascript
   import {
     Controller,
     Get,
     Param,
     Body,
     Post,
     Patch,
     Delete,
   } from "@nestjs/common";

   @Controller("cats")
   export class CatsController {
     @Get()
     findAll(): string {
       return "This action returns all cats";
     }

     @Get(":id")
     findOne(@Param("id") id: number): string {
       return `This action returns a cat with the provided id`;
     }

     @Post()
     create(@Body() body: any): string {
       return `This action returns the body of the cat`;
     }

     @Patch("id")
     update(@Param("id") id: number, @Body() body: any): string {
       return `This action updates the body of the cat`;
     }

     @Delete("id")
     remove(@Param("id") id: number): string {
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

    An Interceptor has a set of useful capabilities which are inspired by the `Aspect Oriented Programming (AOP) technique`.

    Aspect Oriented Programming is a `programming paradigm` that aims to increase `modularity` by allowing the separation of cross-cutting concern.

    Interceptors make it possible to:

    `Binding extra logic before / after method execution:` An Interceptor can execute logic before and after a method is executed. This can be useful for tasks like logging, transforming the result of a method, or handling errors.

    `Transforming the result returned from a function:` An Interceptor can transform the response returned from a method. For example, you could use an interceptor to transform all responses to have a specific format.

    `Handling errors:` An Interceptor can also handle errors thrown within your application. This can be useful for logging or transforming errors before they're sent to the client.
    Here is an example of an interceptor that logs the user interactions as shown in the [Nestjs document](https://docs.nestjs.com/interceptors)

    ```javascript
    import {
      Injectable,
      NestInterceptor,
      ExecutionContext,
      CallHandler,
    } from "@nestjs/common";
    import { Observable } from "rxjs";
    import { tap } from "rxjs/operators";

    @Injectable()
    export class LoggingInterceptor implements NestInterceptor {
      intercept(context: ExecutionContext, next: CallHandler): Observable<any> {
        console.log("Before...");

        const now = Date.now();
        return next
          .handle()
          .pipe(tap(() => console.log(`After... ${Date.now() - now}ms`)));
      }
    }
    ```

    **[⬆ Back to Top](#table-of-contents)**

13. ### What are pipes in the context of NestJS?

    Pipes are a feature of NestJS that allows for validation or transformation of data before it is passed to a route handler and can either return the arguments as is, modify them, or throw an exception.
    A pipe is a class annotated with the `@Injectable()` decorator, which implements the `PipeTransform interface`

    `Validation:` This is the most common use case for pipes. They can be used to validate incoming data to ensure it matches a certain data schema. If the data is invalid, the pipe can throw an exception to prevent the route handler from being executed.

    `Transformation:` Pipes can transform incoming data into a desired format. For example, you might want to automatically convert incoming strings to numbers, or convert an entity's ID into the entity itself.
    Here's an example of a simple pipe that validates and transforms an incoming string into a number:

    ```javascript
    import {
      PipeTransform,
      Injectable,
      ArgumentMetadata,
      BadRequestException,
    } from "@nestjs/common";

    @Injectable()
    export class ParseIntPipe implements PipeTransform<string, number> {
      transform(value: string, metadata: ArgumentMetadata): number {
        const val = parseInt(value, 10);
        if (isNaN(val)) {
          throw new BadRequestException("Validation failed");
        }
        return val;
      }
    }
    ```

    This `ParseIntPipe` is therefore used in this way

    ```javascript

      @Get()
      async findOne(@Query('id', ParseIntPipe) id: number) {
        return this.usersService.findOne(id);
      }

    ```

    Nest comes with nine pipes available out-of-the-box:
    `ParseIntPipe:` This pipe transforms an incoming string into an integer. If the string cannot be parsed into an integer, it throws an exception. As shown above.

    `ValidationPipe:` This pipe validates that the incoming request body matches a specific DTO (Data Transfer Object). If the data is invalid, it throws an exception.

    `ParseFloatPipe:` Similar to `ParseIntPipe`, but transforms an incoming string into a float.

    `ParseBoolPipe:` This pipe transforms an incoming string into a boolean. It accepts 'true' and 'false' as valid boolean strings.

    `ParseArrayPipe:` This pipe transforms a comma-separated string into an array. It can also validate the items in the array if you provide a validation schema.

    `ParseUUIDPipe:` This pipe validates that an incoming string is a valid UUID. If the string is not a valid UUID, it throws an exception.

    `ParseEnumPipe:` This pipe validates that an incoming string is a valid value of a specific TypeScript enum.

    `DefaultValuePipe:` This pipe provides a default value if the incoming value is `undefined` or `null`.

    `ParseFilePipe:` This pipe is used to handle file uploads or parse file data in some way.

    **[⬆ Back to Top](#table-of-contents)**

14. ### What are guards in the context of NestJS?

    Guards are functions that have a single responsibility. They determine whether a given request will be handled by the route handler or not, depending on certain conditions (like permissions, roles, ACLs, etc.) present at run-time. For example, you might use a guard to check if a user is logged in before allowing them to access a route.

    A `guard` is a class annotated with the `@Injectable()` decorator, which implements the `CanActivate` interface. This interface should return a boolean or a Promise that resolves to a boolean. If it returns true, the request proceeds to the route handler. If it returns false, the request is denied and the route handler is not executed.
    Here's an example of a basic guard:

    ```javascript
    import { Injectable, CanActivate, ExecutionContext } from "@nestjs/common";

    @Injectable()
    export class AuthGuard implements CanActivate {
      canActivate(context: ExecutionContext): boolean | Promise<boolean> {
        const request = context.switchToHttp().getRequest();
        // Add your authentication logic here
        // For example, check if a valid JWT token exists in the request headers
        return true; // or false if the request should be denied
      }
    }
    ```

    In this example, AuthGuard allows all requests to proceed. In a real application, you would add your authentication logic in the canActivate method.

    **[⬆ Back to Top](#table-of-contents)**

15. ### What are middlewares in the context of NestJS?

    Middleware is a function which is called before the route handler. Middleware functions have access to the `request` and `response` objects, and the `next()` middleware function in the application’s request-response cycle.

    The next middleware function is commonly denoted by a variable named `next`. Middlewares can be used for a variety of purposes, such as logging, authentication, and authorization. These functions are used to execute any code, make changes to the request and the response objects, end the request-response cycle, or call the next middleware function in the stack.

    Middlewares can perform the following tasks:

    1. Execute any code.
    2. Make changes to the request and the response objects.
    3. End the request-response cycle.
    4. Call the next middleware function in the stack.
       If the current middleware function does not end the request-response cycle, it must call next() to pass control to the next middleware function. Otherwise, the request will be left hanging.
       On how to create a middleware check the [Nestjs Documentation](https://docs.nestjs.com/middleware)

    **[⬆ Back to Top](#table-of-contents)**

16. ### Explain the concept of Dependency Injection in NestJS. How does it help in building modular and testable applications?

    Dependency Injection (DI) is a design pattern in which a class receives its dependencies from external sources rather than creating them itself. This pattern is fundamental to the way NestJS is designed. dependency injection involves letting the framework manage the creation and injection of dependencies into the components (controllers, services, and more) as needed.

    This is achieved through decorators, providers, and the NestJS IoC (Inversion of Control) container
    Here is an example:

    ```javascript
    import { Injectable } from "@nestjs/common";

    @Injectable()
    export class AppService {
      getHello(): string {
        return "Hello World!";
      }
    }
    ```

    ```javascript

      import { Controller, Get } from '@nestjs/common';
      import { AppService } from './app.service';

      @Controller()
      export class AppController {
        constructor(private appService: AppService) {}

          @Get()
           getHello(): string {
            return this.appService.getHello();
          }
      }

    ```

    In this example, `AppService` is a provider that is injected into `AppController` through the constructor. When AppController is created, NestJS automatically creates an instance of AppService and passes it to the constructor.

    `DI` enables us build modular and testable applications in several ways:

    `Modularity:` By injecting dependencies, you can easily swap out one implementation for another. This is useful when you want to change the behavior of parts of your application without changing the classes that use them.

    `Testability:` DI makes it easy to unit test your classes, as you can inject mock versions of dependencies for testing purposes.

    `Separation of Concerns:` Each class focuses on its own behavior, delegating the behavior of its dependencies to the classes that implement those dependencies. This leads to cleaner, more readable code

    **[⬆ Back to Top](#table-of-contents)**

17. ### What’s the difference between @injectable() and @inject() decorators?

    `@Injectable():` This decorator marks a class as a provider that can be managed by the NestJS dependency injection system. It means that NestJS will create an instance of this class and can inject it where it's needed.

    It's typically used on services, which can then be injected into controllers or other services.

    ```javascript
    @Injectable()
    export class CatsService {
      // ...
    }
    ```

    `@Inject():`This decorator is used inside a class to inject a dependency. It's used in the constructor of a class to specify a dependency that should be injected.

    If you're injecting a class provider, you don't need to use @Inject() because TypeScript's reflection system can infer the type. But if you're injecting a non-class provider (like a value or a factory), or if you're working in JavaScript, you need to use @Inject() to tell NestJS what to inject.

    ```javascript
      export class CatsController {
        constructor(@Inject('CatsService') private catsService: CatsService) {}
      }
    ```

    **[⬆ Back to Top](#table-of-contents)**

18. ### How does the Nest logger differ from the standard console.log() and when would you prefer one over the other?

    The `NestJS Logger` provides additional features compared to `console.log()`. It includes context information, supports log levels such as (`log`, `fatal`, `error`,`warn`, `debug`, and `verbose`), and can be customized.

    Use `console.log()` for quick debugging or simple logging needs.

    Use NestJS Logger when you need more control over your logs, such as in larger or production applications. It helps in filtering logs based on levels and provides context, making it easier to trace the source of the log.

    On how the `Nest logger` is implemented checkout [Nestjs Documentation](https://docs.nestjs.com/techniques/logger)

    **[⬆ Back to Top](#table-of-contents)**

19. ### What is the difference between interceptors and middleware?

    In NestJS, both `interceptors` and `middleware` can be used to add extra logic before or after HTTP requests. However, they have some key differences:

    `Interceptors:` have a more comprehensive scope than middleware. They can be used with both HTTP requests and other types of transport like WebSockets and microservices.

    Interceptors can also manipulate the response sent back to the client, for example by transforming the response object, adding extra headers, or changing the status code. They can also be used to implement performance tracking, logging, caching, etc.

    `Middleware:` in NestJS is similar to Express middleware. It's specific to the HTTP request-response cycle and can't be used with other types of transport. Middleware functions have access to the request and response objects, and they can end the request-response cycle or call the next middleware function in the stack.

    They are useful for tasks like logging, error handling, or validating request data.

    In general, if you're working with HTTP requests and you need to add logic that doesn't modify the response sent to the client, middleware can be a good choice. If you need to add logic that applies to other types of transport such as WebSockets and microservices, or if you need to modify the response, use an interceptor.

    **[⬆ Back to Top](#table-of-contents)**

20. ### What testing frameworks work best with NestJS?

    NestJS is a Node.js framework, so any testing framework that works with Node.js will work with NestJS. Some popular options include `Jest`, `Mocha`, and `Jasmine.`
    NestJS is built with testing in mind and it comes with its own testing module called `@nestjs/testing.` This module provides utilities for testing, such as a testing module and HTTP testing utilities.

    **[⬆ Back to Top](#table-of-contents)**

21. ### Explain the purpose of DTOs (Data Transfer Objects) in NestJS.

    DTOs are used to define the structure of data exchanged between different layers of an application. They define the shape of data for a specific operation, such as creating, updating, or returning data.

    DTOs serve several purposes which include:
    `Validation:` With the `class-validator` package, you can add validation rules to the fields in your DTOs. NestJS can automatically validate incoming requests against these rules and return an error if the request is invalid.

    `Documentation:` DTOs provide a clear model of what the data should look like. This can be helpful for other developers, and for tools like Swagger to automatically generate API documentation.

    `Type Safety:` DTOs provide type safety in TypeScript, which can help catch errors at compile time.

    ```javascript
    import { IsString, IsInt } from "class-validator";

    export class CreateCatDto {
      @IsString()
      name: string;

      @IsInt()
      age: number;

      @IsString()
      breed: string;
    }
    ```

    In the above example, CreateCatDto is a DTO that represents the data needed to create a cat. It expects a name and breed of type string, and an age of type number. The @IsString() and @IsInt() decorators are used to apply validation rules.

    **[⬆ Back to Top](#table-of-contents)**

22. ### How can you handle asynchronous operations in NestJS, and what is the role of the Promise object?

    NestJS supports asynchronous operations through the use of the `async` and `await` keywords. When a function returns a Promise, it can be awaited, allowing non-blocking execution. The Promise object represents a value that may be available now, or in the future, or never.

    ```javascript
    import { Injectable } from "@nestjs/common";

    @Injectable()
    export class AppService {
      async getHello(): Promise<string> {
        const result = await someAsyncOperation();
        return `Hello ${result}`;
      }
    }
    ```

    In this example, `getHello()` is an asynchronous method that returns a Promise. The await keyword is used to pause the execution of the function until someAsyncOperation() completes and the Promise is resolved.

    Promises are useful for handling single asynchronous operations. If you need to handle a stream of asynchronous values, you might want to use Observables instead, which are provided by the RxJS library and are also integrated into NestJS.

    **[⬆ Back to Top](#table-of-contents)**

23. ### Explain the purpose of the @InjectRepository() decorator in NestJS.

    The `@InjectRepository()` decorator in NestJS is used to inject a repository instance into a service or controller. It is commonly used with `TypeORM` for database interaction, allowing the injection of repositories for specific entities.

    A repository in TypeORM is a way to manage entities: it provides methods to insert, update, remove, and load entities. By injecting a repository, you can use these methods in your service or controller.

    Here is an example:

    ```javascript
      import { Injectable } from '@nestjs/common';
      import { InjectRepository } from '@nestjs/typeorm';
      import { Repository } from 'typeorm';
      import { User } from './user.entity';

      @Injectable()
      export class UserService {
        constructor(
          @InjectRepository(User)
          private usersRepository: Repository<User>,
        ) {}

        findAll(): Promise<User[]> {
          return this.usersRepository.find();
        }
      }
    ```
    In the above example `@InjectRepository(User)` is used to inject a repository for the `User` entity. This repository is then used in the `findAll` method to load all users.

    **[⬆ Back to Top](#table-of-contents)**

24. ### Explain the purpose of the @nestjs/jwt package in NestJS?
    The `@nestjs/jwt` package is a NestJS module that provides functionality around JSON Web Tokens (JWTs). JWTs are a popular method for handling authentication and authorization in web applications.

    It includes decorators like `@AuthGuard('jwt')` to protect routes with JWT-based authentication and supports the generation and verification of JWTs.

    Here are some of the things you can do with the @nestjs/jwt package:

    `Generate JWTs:` You can create a new JWT with specific payloads and sign it with a secret key.

    `Verify JWTs:` You can verify a received JWT to ensure it's valid and hasn't been tampered with.

    `Decode JWTs:` You can decode a JWT to access the payload information.

    The `@nestjs/jwt` package is often used in combination with the `@nestjs/passport package`, which provides a way to handle authentication in a flexible, modular way. Together, these packages can be used to implement JWT authentication strategy.

     **[⬆ Back to Top](#table-of-contents)**

25. ### Discuss how tokens are used for authorization in an API. What is the difference between authentication and authorization, and how are these processes implemented with tokens?
   Tokens, such as JWTs (JSON Web Tokens), are used for authorization in APIs to ensure that a user has permission to access certain resources or perform certain actions.

   `Authentication` is the process of verifying the identity of a user. When a user logs in with their credentials, the server verifies these credentials and if they are valid, the server generates a token. This token often contains information about the user and is sent back to the client.

   `Authorization` on the other hand, is the process of verifying what a user has access to. Once a user is authenticated and their token is sent with each request, the server can verify the token and check if the user has the necessary permissions to perform the requested action.

   Here's a basic process:

   1. User sends their credentials (like username and password) to the server.
    
   2. Server verifies the credentials. If they're valid, the server generates a token and sends it back to the client.
    
   3. In subsequent requests, the client sends this token in the header of the request.
    
   4. The server verifies the token and checks the user's permissions. If the user has the necessary permissions, the server processes the request.
    
   In this way, tokens serve as proof of authentication and can carry information about user's permissions for authorization. They provide a stateless, scalable solution for securing APIs. 

    **[⬆ Back to Top](#table-of-contents)**

26. ### Why is it important for tokens to have an expiration time? How can you implement token expiration in NestJS, and what role do refresh tokens play in maintaining user sessions?
   Tokens having an expiration time is important for security reasons. If a token is stolen or leaked, it can be used to gain unauthorized access to the system. By setting an expiration time, you limit the time window in which a stolen token can be used.

   In NestJS, you can set the expiration time of a JWT when you sign it using the JwtService. Here's an example:

   ```javascript
      this.jwtService.sign(payload, { expiresIn: '60s' });
   ```

   In this example, the token will expire 60 seconds after it's issued.

   However, having tokens expire can be inconvenient for the user, as they would have to log in again every time their token expires. This is where `refresh tokens` come in.

   **[⬆ Back to Top](#table-of-contents)**