# Hyrum Wright on Software Engineering at Google

TODO: Make sure that you read and understand this example.

## **Sound Check Session: January 8, 2024**

## **Recording Session: January 19, 2024**

## **TL;DR**

- The "Software Engineering at Google" book explores some of the lessons learned
and best practices at Google. This episode interviews Hyrum Wright, one of the
editors of and contributors to this book.

- **Guest: Hyrum Wright, Senior Staff Engineer at Google**

- **Note: the book is available to read for free at:
https://abseil.io/resources/swe-book/html/toc.html**.

## Introduction to the Show (2 Minutes)

- Welcome to Software Engineering Radio, I'm your host Gregory M. Kapfhammer.
Today's guest is Hyrum Wright, a Senior Staff Software Engineer at Google and
the co-author of the book called "Software Engineering at Google."

- Hyrum leads the Code Health Team that is responsible for the maintainability
of Google's source code, ensuring the scalable evolution of billions of lines of
code. Along with being a visiting lecturer at Carnegie Mellon University, Hyrum
was an editor of and contributor to the "Software Engineering at Google" book.

- Welcome to Software Engineering Radio, Hyrum!

## Setting the Stage: Introduction to the Book (10 Minutes)

- **Goal**: introduce some of the key insights from the book and set the stage
for an in-depth discussion of specific chapters of the book.

- Amazon reports that, for those people who read the book on the Kindle
platform, there are two sentences that readers highlight most frequently. To
give listeners some insight into the type of software engineering content that
they will find in the book, I'm going to read you a quote and ask you to explain
what it means:

   - **Quote 1**: "With a sufficient number of users of an API, it does not matter
   what you promise in the contract: all observable behaviors of your system
   will be depended on by somebody."

   - **Quote 2**: "Traditional managers worry about how to get things done,
   whereas great managers worry about what things get done (and trust their team
   to figure out how to do it)."

- The book contains both "technical" (e.g., software testing) and "professional"
(e.g., project management) content. Follow-on questions:

   - Who is the audience for this book?
   - Why did you and your co-authors focus on both of these areas?
   - What is a key takeaway from the book?

- At its outset, the book points out that "software engineering" is different
from "programming". Follow-on questions:

   - What do these terms mean?
   - How are they similar to and different from each other?
   - Can you distinguish these terms using a concrete example from your work at
   Google?

## Professional Principles at Google (20 Minutes)

- **Goal**: explore the professional principles that guide software engineering
  at Google (roughly, Chapters 1 through 14 of the book).

- The book talks about "scale and efficiency challenges" in areas like upgrading
the programming languages and compilers at Google. Questions:

   - What challenges has Google faced in these areas?
   - What are some practical strategies for solving these challenges at scale?
   - Since the book was published, have new scale challenges arisen?
   - If so, how have you applied the book's principles to handle them?

- A significant portion of the book explains the strategies that Google employs
to ensure that software engineers work well in teams and share knowledge
effectively. Many of these principles are summarized with catchy phrases! What
do they mean? Can you illustrate them with a concrete example?

   - "The Genius Myth"
   - "Hiding Considered Harmful"
   - "Being Googley"

- Google has invested significant time and effort to measure "engineering
productivity". This leads to the following questions:

   - Why is it important to measure engineering productivity?
   - How do you use "goals" and "signals" to measure productivity?
   - In the context of Google's Code Health team that you lead, how do you
   measure productivity?

   Listeners who want to learn more about how to measure engineering productivity
   are encouraged to check out SE Radio Episode 317:

   https://www.se-radio.net/2018/02/se-radio-episode-317-travis-kimmel-on-measuring-software-engineering-productivity/

- Google has adopted several processes for reviewing code and ensuring that it
adheres to specific style guides and rules. Follow-on questions:

   - Can you give an example of a style guide that Google adopted?
   - How do you enforce adherence to this style guide?
   - What are the best practices for code review at Google?

## Technical Best Practices at Google (30 Minutes)

- **Goal**: explore the technical principles that guide software engineering at
Google (roughly, Chapters 15 through 30 of the book).

- You and Titus Winters gave a talk at CppCon with the tongue-in-cheek title:
"All Your Tests are Terrible: Tales from the Trenches". Why were the tests at
Google so "terrible"? What are the characteristics of "good" and "bad" tests at
Google?

- Several chapters in the book talk about both the importance and limitations of
automated testing at Google. Let's talk about this in greater detail:

   - Google encourages developers to write the "smallest possible test" for a
   source code component. Why? What are the benefits and drawbacks of this
   approach?
   - The book asserts that "flaky tests are expensive". What is a flaky test?
   Why are they expensive? How does Google handle flaky test cases?
   - Software engineers often measure the adequacy of their test suite through
   code coverage. At Google, what is code coverage and how do you use it?
   - Google's software engineers sometimes use "test doubles". What is a test
   double? What are the trade-offs associated with using them at Google?

   The archives of Software Engineering Radio feature numerous episodes on
   software testing. Listeners who want to learn more are invited to check out
   recent Episodes 595 on "Approval Testing" and 572 on "Flaky Tests":

   - https://www.se-radio.net/2023/12/se-radio-595-llewelyn-falco-on-approval-testing/
   - https://www.se-radio.net/2023/07/se-radio-572-greg-kapfhammer-on-flaky-tests/

- The book describes Google's static analysis platform called Tricorder.
Follow-on questions:

   - What is static analysis?
   - What are the benefits and limitations of static analysis at Google?
   - How and when do Google's software engineers use Tricorder?

- You were the author of the chapter on "Large-Scale Changes" at Google and
you've authored research papers in this area. Let's talk about this topic in
greater detail!

   - What is a large-scale change? Why do you make them?
   - How do engineers implement large-scale changes to Google's code base?
   - Can you give an example of a large-scale change that you have made?
   - How did you ensure that the large-scale change was correct?

- This episode has overviewed many of the strategies that Google's engineers
adopt to create great software. Listeners who want another take on software
engineering best practices are encourage to try Episode 430 on "Seriously Good
Software":

   - https://www.se-radio.net/2020/10/episode-430-marco-faella-on-seriously-good-software/

## Conclusion, Thanks, and Goodbye! (3 Minutes)

- This episode covered many lessons cataloged in "Software Engineering at
Google" book. Is there anything else about the book that you wanted to
highlight?

- As we draw this episode of Software Engineering Radio to a conclusion, do you
have a call to action for our listeners?

- Hyrum, thanks for taking the time to chat with the listeners of Software
Engineering Radio. This has been an entertaining and informative conversation!
If you are a listener who wants to learn more about Software Engineering at
Google, please check the show notes for references and additional details. Okay,
this is Gregory Kapfhammer signing off for Software Engineering Radio. Goodbye!

## Logistics

- Zencastr Recording Session: https://recording.zencastr.com/seradio/software-engineering-at-google-with-hyrum-wright
