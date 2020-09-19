# <div align="center">CellularJS</div><div align="center"><sub>A framework to grow from zero to big</sub></div><sub style="color: red">🐘</sub>

## 1. Abstract
CellularJS is a hybrid microservices framework. The main purpose of the framework is providing flexible scalability for software development, or you can say, better developer experience.

## 2. Hybrid architecture
CellularJS is not only about code, but also come with strategy to help you grow from zero to big, and that strategy is supported by hybrid architecture.

Technically, hybrid architecture or hybrid microservices can be monolithic or a combination of monolithic and microservices, it all depends on your needs. The idea behind hybrid architecture is starting with small stuff then grow it up on demand. By deferring the need for dramatic performance scalability at early stage, you will have more time to concentrate on other valuable things.

## 3. How it come true
At the heart of CellularJS are many stuffs got inspiration from Domain Driven Design(DDD).
- From Anti-Corruption Layer, it is "message": Services, no matter green or brown, when they want to talk to each others they must use a same language. In CellularJS, the language is implemented as internal request/response.
- From Bounded Context and Aggregate Root, it is "flow": It is ugly if a service access directly into internal of other service for changing state or anything else. For better management, it is only allowed to access via public API.

All of above theories will have nothing special if you choose microservices as development method. The natural physical isolation characteristic of microservices will help you detect bounded context violation easier. Hybrid architecture, because of lack of this isolation, is fragile. Thus, you need to have strong theory to guide you.

Beside of a good theory like DDD, you also need tool too. You can consider CellularJS as a tool that enhance isolation by programmatic way. CellularJS create a programmatic network where cells(same as services) can communicate with each others via a message flow. It use concept of "space" to specify cells relationship and use appropriate driver for communication.

With the help of programmatic network, your services will become protocol-agnostic. No matter the driver use function call, HTTP, or AMQP, you will get the same message and your domain logic will be safe from protocol chaos. As a result, you can break your services up into multiple physical isolation services more easily(If you really need it XD).

One more time, hybrid architecture is fragile, you need a good theory to follow. CellularJS is about programmatic isolation tool, **NOT** a physical one.

Happy coding 💕

## 4. Resources
Protocol-agnostic is one of many spheres that make hybrid architecture easier. As usual, you will need more things like transaction across boundaries, project skeleton, ... For more resources, please visit [cellularjs.com](#).

## 5. Contributor
Do you interested in CellularJS? Have a look at [contributor guideline](#).