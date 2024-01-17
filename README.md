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
| 1   | [What is Nestjs](#what-is-nestjs)                                         |
| 2   | [How to declare a class as a controller in Nest.js](#How-to-declare-a-class-as-a-controller-in-Nest.js)  
| 3   | [What is the main responsibility of controllers](#What-is-the-main-responsibility-of-controllers)  
| 4   | [Can you explain how to use decorators in a NestJS controller?](#Can-you-explain-how-to-use-decorators-in-a-NestJS-controller?) 


### Answers


1. ### What is Nestjs

   Nest(NestJS) is a framework for building efficient, scalable Node.js server side applications. It uses progressive JavaScript and its built with and fully suports Typescript.

2. ### How to declare a class as a controller in Nest.js

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

3. ### What is the main responsibility of controllers

   Controllers are responsible for handling incoming `requests` and returning `responses` to the client.Controllers organize routes and handle HTTP requests that come to those routes.
   
   **[⬆ Back to Top](#table-of-contents)**

4. ### Can you explain how to use decorators in a NestJS controller?
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