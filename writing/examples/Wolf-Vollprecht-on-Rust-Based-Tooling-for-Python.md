# Wolf Vollprecht on Rust-Based Tooling for Python

TODO: Make sure that you read and understand this example.

## **Sound Check Session: End of January / Start of February**

## **Recording Session: Middle / End of February**

### **TL;DR**

This episode explores Rust-based tooling for Python through the lens of Python
package management tools like Pixi.

**Guest: Wolf Vollprecht, CEO of Prefix.dev and Co-Creator of the Pixi Package Manager**

### Introduction to the Show (2 Minutes)

- Welcome to Software Engineering Radio, I'm your host Gregory M. Kapfhammer.
Today's guest is Wolf Vollprecht, the CEO and founder of Prefix.dev. He is the
creator of both the mamba package manager, implemented in C++, and the Pixi
package manager implemented in Rust. Wolf is also the creator of numerous
packages on conda-forge, a core member of the conda-forge team and the founder
of the RoboStack project. Welcome to Software Engineering Radio, Wolf!

- During this episode we will talk with Wolf about the Pixi package manager and
other Rust-based tooling for the Python programming language. Before we get to
the main topic let's set the stage by discussing package management in Python!

### Setting the Stage: Basics of Package Management (10 Minutes)

- **Goal**: explore Rust-based tooling for Python through the lens of package
management management tools for Python. Set the stage by explaining
package management fundamentals for (mostly) the Python programming language.

- There are numerous package management tools for the Python programming
language. Start by exploring the basics of package management in Python:

    - Can you give an example of what a package manager does for a Python developer?
    - At a high level, how does package management work in Python?
    - Briefly explain each of the following package managers:
        - pip and pipx
        - pipenv and poetry
        - conda and mamba
    - **Note**: these tools are group together by their similarities and differences
    - What programming languages are used to implement these tools?
    - Which of these tools are specific to Python? Suitable for other languages?

- What are some of the challenges that a programmer may face when using these
package management tools? Why do they face these challenges?

- Listeners who want to learn more about package management are encouraged to
check out Episode 489, "Sam Boyer on Package Management" and Episode 509, "Matt
Butcher and Matt Farina on Helm Charts".

    - References:
        - https://www.se-radio.net/2021/12/episode-489-sam-boyer-on-package-management/
        - https://www.se-radio.net/2022/04/episode-509-matt-butcher-and-matt-farina-on-helm-charts/

### Package Management in Pixi: Rust-Based Tooling for Python (25 Minutes)

- **Goal**: explore the features of Pixi and how it is implemented in Rust.
Ensure that the listener can see how Pixi addresses the challenges that were
highlighted at the end of the episode's previous section.

#### Overview of Pixi's Features

- Before diving into the details, it is important to note that you implemented
Pixi in the Rust programming language. At a high level, why did you decide to
implement Pixi in Rust?

- Description of Pixi from pixi.sh: "It allows the developer to install
libraries and applications in a reproducible way. Developers can use pixi in a
cross-platform fashion on Windows, Mac, and Linux." Quick follow-on questions:

    - What is the difference between a "library" and an "application"?
    - What is the meaning of "reproducible" in this context?
    - What about pixi allows it to work in a "cross-platform" manner?

- The pixi.sh site also explains that the tool should provide an "isolated
environment" for an application or a library. What does this mean in the context
of Python programming?

- Are there any other key features of Pixi that you would like to highlight?

#### Key Features of Pixi and Comparison to Related Tools

- Can you give a concrete example of a programming task that is hard for a
developer to do with a tool like poetry or pipenv but is easier to do with Pixi?

- Summary of the basic features provided by Pixi:

    - Initialize a project
    - Add project dependencies
    - Add a task and execute it
    - Run a program managed by Pixi

    Follow-on questions:

    - How does a developer perform each of these steps with Pixi?
    - Can you sketch the way in which you implemented Pixi to perform each of
    these steps?

- Pixi is different from a package manager like poetry or pipenv because it can
actually bundle the Python language itself. Follow-on questions:

    - Why is this a useful feature for a package manager?
    - How does Pixi implement this feature?
    - How does this compare to the use of tools like nix, asdf, or rtx?
    - **Note:** Nix is a package manager in NixOS. Next, asdf is a runtime
    environment manager normally used to install programming languages. Finally,
    the rtx runtime executor, that is compatible with and operates like asdf, is
    also implemented in the Rust programming language.

#### Implementing Pixi in Rust

- Now that we have explored the main features provided by Pixi, can you explain
further why you decided to implement Pixi in Rust? What is an example of a Pixi
feature that is easier (or more feasible) to implement in Rust than in Python?

- A comparison table in the Pixi FAQ explains that it is fast and that tools
like Poetry and Conda are not fast. What is the meaning of the "fast" adjective
in this assertion? What about Pixi's Rust-based implementation makes it fast?

- Listeners who want to learn more about Rust can explore Episode 490, "Tim
McNamara on Rust" and Episode 562, "Bastian Gruber on Rust Web Development".

    - References:
        - https://www.se-radio.net/2021/12/episode-490-tim-mcnamara-on-rust-2021-edition/
        - https://www.se-radio.net/2023/05/se-radio-562-bastian-gruber-on-rust-web-development/

### Rust-Based Tools that Support Pixi (15 Minutes)

- **Goal**: explore the Rust-based tools that support Pixi's main features.

- rattler-build tool:

    - The GitHub repository for rattler-build describes the tool in the
    following fashion: "The rattler-build tooling and library creates cross-platform
    relocatable binaries / packages from a simple recipe format." Questions:

    - Can you explain more about how rattler-build works?
    - How does rattler-build support creating cross-platform binaries for Pixi?
    - This tool currently creates packages for conda-forge. Would it be possible
      for it to also create packages for distribution through PyPI?
    - What notable features of Rust are used by the rattler-build tool?

- rip tool:

    - The GitHub repository for rip describes the tool in the following fashion:
    "rip is a library that allows the resolving and installing of Python PyPI
    packages from Rust into a virtual environment". Follow-on questions:

    - Can you explain more about how rip works?
    - What are the similarities and differences between rip and the following
    Python-based tools:
       - pip
       - pipx
       - pipenv
       - poetry

    - The description of rip mentions that it uses "aggressive caching of PyPI
    metadata" What is this type of caching and why is it needed and useful?

    - Rip also uses the Rust-based Resolvo package. Questions:
        - Resolvo performs constraint solving. Can you give a concrete example
        of why this is needed in the context of Rip?
        - How does Resolvo perform constraint solving?
        - How does Resolvo support incremental and/or lazy constraint solving?

- Listeners who want to learn more about Python programming can explore Episode
431, "Ken Youens-Clark on Learning Python". Reference:
https://www.se-radio.net/2020/10/episode-431-ken-youens-clark-on-learning-python/.

- More details about another Rust-based program are available in Episode 581,
"Zach Lloyd on Terminal Emulations. Reference:
https://www.se-radio.net/2023/09/se-radio-581-zach-lloyd-on-terminal-emulators/.

### Lessons Learned from Building Rust-Based Tooling for Python (5 Minutes)

- **Goal**: briefly explore the lessons learned from building Rust-based tools
for Python developers, identifying key features of Rust to support this task.

- What are the key features of the Rust programming language and the Rust
ecosystem that make it ideal for implementing programs like Pixi, rattler-build,
and rip?

- Are there any drawbacks to implementing Python tooling in Rust?

- What advice would you give to a programmer who wants to implement a Python
tool in the Rust programming language?

### Conclusion, Thanks, and Goodbye! (3 Minutes)

- We've covered many interesting aspects associated with implementing tools like
Pixi in Rust. Are there additional topics that we should discuss?

- As we draw this episode of Software Engineering Radio to a conclusion, do you
have a call to action for our listeners?

- Wolf, thanks for taking the time to chat with the listeners of Software
Engineering Radio. This has been an awesome conversation! If you are a listener
who wants to learn more about programming in Rust or Python, please check the
show notes for references and additional details. Okay, this is Gregory
Kapfhammer signing off for Software Engineering Radio. Goodbye!
