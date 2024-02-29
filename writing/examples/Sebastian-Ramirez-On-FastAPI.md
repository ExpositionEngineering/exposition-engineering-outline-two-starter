# Sebastian Ramirez on FastAPI

TODO: Make sure that you read and understand this example.

## **Sound Check Session: Soft Booked, January 2024**

## **Recording Session: Soft Booked, February 2024**

## **TL;DR**

FastAPI enables the creation of a web-based API in the Python programming
language. This episode will explore the key characteristics of FastAPI, how it
was implemented, and how it is similar to and different from other approaches
to creating APIs in the Python programming language. It will also explain how
to create and deploy a FastAPI implemented in Python.

- **Guest: Sebastian Ramirez, Creator of FastAPI**

## Introduction to the Show (2 Minutes)

- Welcome to Software Engineering Radio, I'm your host Gregory M. Kapfhammer.
Today's guest is Sebastian Ramirez, the creator of FastAPI and Typer and several
other open-source software tools for the Python programming language. Sebastian
is a Senior Staff Engineer at Forethought and an Open-Source Fellow at Sequoia
Capital. Sebastian has extensive experience at building custom software
applications that involve APIs, data processing, distributed systems, and
machine learning. Welcome to Software Engineering Radio, Sebastian!

- During this episode we will talk about FastAPI. Let's start by exploring what
FastAPI is and the problem that it solves.

## Setting the Stage: Introduction to FastAPI (10 Minutes)

- **Goal**: introduce what FastAPI is and how it helps Python developers to
create an application programming interface (API).

- The FastAPI website describes the tool in the following fashion: "FastAPI is a
modern, fast (i.e., high-performance), web framework for building APIs with Python
3.8+ based on standard Python type annotations." Follow-on questions:

    - What can a Python developer build with FastAPI?
    - At a high level, what are the key features of FastAPI?
    - Can you briefly share a success story associated with the use of FastAPI?

- Before diving into the details about FastAPI, let's explore how some API terms
connect to FastAPI:
   - OpenAPI Standard:
      - Does FastAPI support the creation of APIs that conform to this standard?
   - Web Server Standards:
      - WSGI (Web Server Gateway Interface)
      - ASGI (Asynchronous Server Gateway Interface)
      - Does FastAPI support the creation of both types of APIs?
   - Web API Standards:
      - REST API
      - GraphQL API
      - Does FastAPI support the creation of both types of APIs?

## Implementation of the Fast API Framework (30 Minutes)

- **Goal**: investigate how FastAPI is implemented in the Python language

- Explore some of the key features provided by FastAPI:

   - FastAPI has automatic API documentation through the use of packages called
   SwaggerUI and ReDoc. What are these packages and how do they work?
   - When a developer adds type annotations to their Python program, FastAPI
   processes them to support developer productivity. How does FastAPI extract
   these annotations and use them to help developers?
   - FastAPI performs input conversion from JSON to Python data types and output
   conversion from Python data types to JSON. How is this implemented?

- FastAPI relies on several other packages in order to achieve its goals:

   - Uvicorn: an ASGI server
      - What are the key features of Uvicorn?
      - How does Uvicorn help to make FastAPI fast from a performance perspective?

   - Starlette: a web micro-framework
      - What are the key features of Starlette?
      - Why does FastAPI use Starlette as part of its foundation?

- FastAPI also uses Pydantic for input validation. Follow-on questions:

   - What are the key features of Pydantic? How does FastAPI use them?
   - Version 2.0 of Pydantic was implemented in Rust. How does this
   re-implementation of Pydantic improve the performance of FastAPI?

- FastAPI and its dependencies aim for high-performance by leveraging both
concurrency and parallelism. Can you give an example to illustrate these
terms and then explain how they are evident in FastAPI's implementation?

- Briefly compare and contrast FastAPI with other Python-based frameworks for
API creation:

    - Django and Django-REST
    - Flask and Flask-based REST frameworks like Marshmallow
    - How are these frameworks similar to and different from FastAPI?

- How does FastAPI support API security through authentication and authorization?

- Listeners who want to learn more about API security are encouraged to check
out Software Engineering Radio Episode 383, "Neil Madden on Securing Your API".

   - Reference:
      - https://www.se-radio.net/2019/10/episode-383-neil-madden-on-securing-your-api/

- Are there any other key features of FastAPI that you would like to highlight?

## Designing, Implementing, and Testing a FastAPI in Python (10 Minutes)

- **Goal**: explore how to use FastAPI to create an API in Python

- Can you overview the high-level steps that a developer takes to create a FastAPI?

- Once a developer has created a FastAPI how do they test and then deploy it?

- What is an example of a well-known Python program that uses FastAPI? Can you
give a concrete example of how it uses FastAPI?

- Listeners to Software Engineering Radio who want to learn more about how to
design and test APIs are encouraged to listen to Episode 387, "Abhinav Asthana
on Designing and Testing APIs" and Episode 542, "Brendan Callum on
Contract-Driven APIS". For more details, please check the show notes!

   - References:
      - https://www.se-radio.net/2019/11/episode-387-abhinav-asthana-on-designing-and-testing-apis/
      - https://www.se-radio.net/2022/12/episode-542-brendan-callum-on-contract-driven-apis/

## Lessons Learned from Building and Testing FastAPI (10 Minutes)

- **Goal**: briefly explore the lessons learned from the guest's experiences
with building FastAPI in the Python language

- The documentation for FastAPI points out that its code base is "100% type
annotated" and that the test suite has "100% test coverage".

    - What is the meaning of these two phrases?
    - What motivated you to pursue these goals?
    - How does the achievement of these goals influence the implementation of
    new features and/or the maintenance of the FastAPI code base?

- As I mentioned at the start of the show, you have successfully created several
other open-source software tools beyond FastAPI. Follow-on questions:

    - Are there any lessons that you have learned about creating software
    frameworks that enhance developer productivity?
    - How have your experiences with FastAPI influenced the ways in which you
    implement other Python packages?

- What advice would you give to a programmer who wants to implement an API
creation tool, like FastAPI, for the Python programming language?

## Conclusion, Thanks, and Goodbye! (3 Minutes)

- In summary, this episode covered the following topics about FastAPI:

    - Key concepts for APIs and FastAPI
    - Implementation of the FastAPI framework
    - Strategies for creating and testing a FastAPI

- Are there additional topics that we should briefly discuss?

- As we draw this episode of Software Engineering Radio to a conclusion, do you
have a call to action for our listeners?

- Sebastian, thanks for taking the time to chat with the listeners of Software
Engineering Radio. This has been an awesome conversation! If you are a listener
who wants to learn more about API creation with Python, please check the show
notes for references and additional details. Okay, this is Gregory Kapfhammer
signing off for Software Engineering Radio. Goodbye!

## Logistics

- Zencastr Recording Session: https://recording.zencastr.com/seradio/sebastian-ramirez-on-fast-api
- Google Meet Link: https://meet.google.com/tov-uxcx-xgh
