Back in 1997 no developer had herd the term of Test Driven Development or TDD for short, they would just write simple throw away code to test the main functionality of the code or just wing it most of the times.

Nowadays there are automated testing frameworks and unit testing has become a mandatory skills on developers resumes.

The Agile and TDD movements have encouraged many programmers to write automated unit tests, and more are joining their ranks every day. But in the mad rush to add testing to our discipline, many programmers have missed some of the more subtle, and important, points of writing good tests.

TDD requires you write tests first and if those tests pass only then you can write that code in production.

TDD also has three major laws that every developer should focus on:

- You may not write production code until you have written a failing unit test.
- You may not write more of a unit test than is sufficient to fail, and not compiling is failing.
- You may not write more production code than is sufficient to pass the currently failing test.

These laws lock you into an never ending cycle of writing tests, after a while these tests may out number the production source code which could be a management disaster.

If you don't write unit tests to test out your code than it's not a big problem but if you write unit tests with the mindset that your tests should be quick and dirty or Just works kind of tests than no testing is better than these tests.

The problem is that tests must change as the production code evolves. The dirtier the tests, the harder they are to change. 

The more tangled the test code, the more likely it is that you will spend more time cramming new tests into the suite than it takes to write the new production code.

It is unit tests that keep our code flexible, maintainable, and reusable. The reason is simple. If you have tests, you do not fear making changes to the code! Without tests every change is a possible bug.

You tests should be easily readable and have the same thing that makes all code readable: clarity, simplicity, and density of expression.

Like a function is supposed to only perform one thing, A single test should only test one part or component of the code. This will further help in keeping things cleaner.

## First Principle

If you want to write clean and efficient tests than follow these five principles:

- Tests should be fast. They should run quickly.
- Tests should not depend on each other. One test should not set up the conditions for the next test.
- Tests should be repeatable in any environment. You should be able to run the tests in the production environment, in the QA environment.
- The tests should have a boolean output. Either they pass or fail. You should not have to read through a log file to tell whether the tests pass.
- The tests need to be written in a timely fashion. Unit tests should be written just before the production code that makes them pass.