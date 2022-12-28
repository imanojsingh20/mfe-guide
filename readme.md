# Micro Frontend

![showcase-mfe][3]

[Source][1]

Micro Frontend architecture is vaguely inspired by Micro-services architecture. Micro frontend architecture is an approach to developing web application as a composition of small frontend apps. Instead of writing a large monolith frontend application, the application is broken down into domain specific micro frontends, which are self-contained and can be developed and deployed independently.

> #### "An architectural style where independently deliverable frontend applications are composed into a greater whole"

## Key Benefits of Micro Frontend Architecture

-   Better scalability.
-   Faster development, as teams can work independently.
-   You can use multiple frameworks in your application. However, it should be done mindfully and transparently to avoid confusion.
-   Deployment independence. The delivery of your micro frontend will not affect the entire application. The changes will affect precisely that part of the business process that it has covered.
-   With micro frontends, you can upgrade, update, or even rewrite parts of the frontend more smoothly than was previously possible.
-   It’s easier to ensure that rest of the app remains stable, as it’s independent. With micro frontends, you no longer need to keep track of the whole app.
-   Codebases are smaller and more manageable.
-   Easier hiring of experts. With micro frontends, you look for professionals to work on a specific part of an app where a particular tech stack is used, so you do not need them to know technologies that other teams use.
-   Easier testing, as you test just separate features.

## Down-sight of Micro Frontend Architecture

-   There must be a special attention to shared libraries between applications, so the browser won't download the same lib multiple times.
-   Code redundancy: some code may be repeated on each application. We surely could write a helper application that others use, but that would create a tight coupling between them.
-   Architectural complexity: it's way easier to manage a single monolith than multiple applications. To overcome this, there must be some automation and a lot of documentation to help developer experience.

The idea behind Micro Frontends is to think about a web app as a composition of features that are owned by independent teams. Each team has a distinct area of business it cares about and specialises in. A team is cross-functional and develops its features end-to-end, from database to user interface.

## Monolithic Frontends

![showcase-mfe-2][5]

## Organisation in Verticals

![showcase-mfe-2][4]

[Source][2]

## The main Concept behind Micro Frontend Architecture is as follows -

-   Be Technology Independent
    Each team should choose and upgrade the stack without coordinating with other teams. Custom elements help to hide implementation details while providing a neutral interface to others.
-   Isolate Team Code
    Never share a runtime, even if teams use the same framework. Build an independent application self-contained. Do not rely on shared state or global variables.
-   Create Team Prefixes
    Use naming conventions where isolation not possible yet. Namespace CSS, Local Storage, Events, and Cookies to avoid collisions and clarify ownership.
-   Favor Native Browser Features over Custom APIs
    Instead of building a global PubSub system, use browser events for communication. If there is a need to build a cross-team API, try to keep it as simple as possible.
-   Build a Resilient Web design
    The features should be useful, even if JavaScript unable to execute. To improve perceived performance, use universal rendering and progressive enhancement.........

<!-- Links to refrences -->

[1]: https://www.cuelogic.com/blog/micro-frontends-part1
[2]: https://micro-frontends.org/

<!-- Links to images -->

[3]: https://www.cuelogic.com/wp-content/uploads/2020/11/01-Gif-1536x864.gif.webp
[4]: https://micro-frontends.org/ressources/diagrams/organisational/verticals-headline.png
[5]: https://micro-frontends.org/ressources/diagrams/organisational/monolith-frontback-microservices.png
