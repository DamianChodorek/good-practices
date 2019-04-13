[Toward Simplifying Application Development, in a Dozen Lessons](http://melconway.com/Home/pdf/simplify.pdf)

### Clean Architecture
- Architecture reflects organisational communication model, reverse is true.
- When teams aren't aware of their architecture (don't have the big picture), it tends to degrade.
- The goad of software architecture is to minimaze the human resources required to build and maintain the required system.
- The measure of design quality is the measure of effort required to meet the needs of the customer.
- All non-trivial abstractions, to some degree, are leaky.
- SOLID - applies to method/class/module/service level
    - Single responsibility principle - one should have only a single responsibility.
    - Open/closed principle - open for extension, but closed for modification.
    - Liskov substitution principle - one should be replaceable with instances of its subtype without altering the correctness of that program.
    - Interface segregation principle - many client-specific interfaces are better than one general-purpose interface.
    - Dependency inversion principle - one should depend upon abstractions, not concretions.
- Importance
    - Composition over inheritance.
    - Convention over configuration.
    - Principle over practices.
    - Simplicity over familiarity.
    - Explicit over magic.
    - Duplication over poor abstraction.
- Packaging principles
    - Screaming Architecture - project structure should tell us very clearly what the system is about, not what framework is used.
    - Go for High Cohesion (group items with functions that are similar in many aspects).
    - Go for Low Coupling (a module is said to be loosely coupled if a module is independent of any other modules).
    - The Release Reuse Equivalency Principle - the granule of reuse is the granule of release.
    - The Common Closure Principle - classes that change together are packaged together.
    - The Common Reuse Principle - classes that are used together are packaged together.
    - The Acyclic Dependencies Principle - the dependency graph of packages must have no cycles.
    - The Stable Dependencies Principle - depend in the direction of stability.
    - The Stable Abstractions Principle - abstractness increases with stability.
- Separate
    - Stable from unstable.
    - Permanent from temporary.
    - Synchronous from asynchronous.
    - Similar from different.
    - Symmetrical from asymmetrical.
    - Construction from operation.
    - Content from presentation.
    - Easy from complex.
    - Stateless from stateful.
    - Application-level code from system-level code.
    - Methods that read from methods that write.
    - One from Many, Many from Many.
- Scalability
    - DRY
    - YAGNI - don’t write code until you actually need it, and remove any code that isn’t being used.
    - Ignorance limits on ability of a software to scale.
    - Good enough for each part is often best for the whole system.
    - Group together things that change at the same time for the same reasons.
    - Legacy code is a code without tests.
    - Adopt "fits in my head" principle.
    - Smaller is not necessarily better, more replaceable is better.
    - Be only as generic as you know you need to be right now.
    - Restrict the scope of data to the smallest possible
    - Complexity is a prison; simplicity is freedom.

### Code readability
- Write boring code.
- Dad code comes from ignorance, not from evil. Don't ignore things.
- Leave code in a better state than it had been before you got it.
- Change one thing at a time.
- Comments should explain why the code is doing something, not what it is doing.
- If you run into an unfixable complexity outside of your program, put a wrapper around it that is simple for other programmers.
- There is no perfect design, there is only a better design.
- A good programmer should do everything in his power to make what he writes simple for other programmers to use and comprehend.
- Everybody who writes software is a designer.
- The best design is the one that allows for the most change in the environment with the least change in the software.
- The ease of maintenance of any piece of software is proportional to the simplicity of its individual pieces.
- Many difficult design problems can be solved by simply drawing or writing them out on paper.
- To handle complexity in your system, redesign the individual pieces in small steps.
- Make it run, make it right, make it fast.
- A method should be a command or a query, but not both. Command modifies the state and doesn't return value. Query doesn't modify the state but returns a value.

### Testing
- A test without an assertion is not a test.
- The overall goal of testing is then to gain valid knowledge about the system.
- FIRST
    - Fast
    - Isolated/Independent
    - Repeatable
    - Self-Validating
    - Thorough

### Errors and bugs
- Fail fast.
- Badly designed systems tend to poison systems they interact with.
- Flexibility breeds bugs.
- Never ignore errors.
- Presence of errors indicates that you don't understand your system well enough.
- Make a clear distinction between critical and non-critical errors.
- Every assert becomes a proper error handling eventually.
- Add logging and error handling early.
- Assume no coincidences, investigate.
- Adress problem directly, not with workaround.
- Most mistakes in software design result from assuming that you will need to do something (or never do something) in the future.
- The world of computers is full of things that should have been strict from the beginning, and became ridiculously complex because they weren't (HTML).
- Bugs most commonly come from somebody's failure to reduce complexity. Less commonly, they come from a misunderstanding of something that was actually simple.
- When solving a problem in a codebase, you're not done when the symptoms stop. You're done when the problem has disappeared and will never come back .
- Debugging is accomplished by gathering data until you understand the cause of the problem.

### Process
- Rather than trying to find extraordinary people to do a job, design the job so that ordinary people can do it well.
- Start small, then extend.
- Everything takes longer than you think.
- Complexity and technology investment is a function of time, so we should revisit theese decision periodically.
- Deployment/monitoring/testing/analysis is first class consideration.
- Whatever the problem is, there's always a right way to solve it.
- It is more important to reduce the Effort of Maintenance than it is to reduce the Effort of Implementation.
- The only time you should seriously consider ditching backwards-compatibility is when keeping it is preventing you from adding obviously useful and important new features.
- The way to measure the productivity of a developer is to measure the product that they produce.
- Your first goal is to get the system into a place where it's getting better over time, instead of getting worse.
- The best way to get real security in things is simplicity.
- Make features easy to use; don't make them unnecessary flexible.
- Humans should dominate machines, business logic should dominate systems.
- All you have to do to succeed in software is to consistently suck less with every release.
- If you're not sure how to write even that core code yet, then just start with the code you are sure about.
- When you're truly clever, what will show up for users is that your program is awesome. It's so awesome, the user hardly notices it's there. That is true brilliance.
- The desirability of a change is directly proportional to the value now plus the future value, and inversely proportional to the effort of implementation plus the effort of maintenance.
- The quality level of your design should be proportional to the length of future time in which your system will continue to help people.
- The longer your program exists, the more probable it is that any piece of it will have to change.
- You can determine whether or not a technology is “bad” by looking at its survival potential, interoperability, and attention to quality.
- The difference between a bad programmer and a good programmer is understanding.
- Its harder to build great team than a great project. Make your team  squad independent of projects.
