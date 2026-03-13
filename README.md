
# autotest: Autonomous Test Agents

Autotest is an experiment in building self-improving AI agents that autonomously generate, maintain, and optimize unit tests for codebases. Inspired by the vision of fully automated research and development, autotest agents operate in iterative loops, continuously analyzing code, running tests, and evolving the test suite without human intervention.

## What is it?

Autotest is a collection of scripts and agents that use GitHub Copilot CLI to:

- Generate new unit tests for your codebase
- Analyze test results and coverage
- Refactor and improve existing tests
- Fix broken tests and adapt to code changes
- Self-edit and optimize their own logic
- Operate within repository constraints and rules

The goal is to create a feedback loop where agents autonomously build, test, and improve code, pushing towards robust, well-tested software.

## How does it work?

The main script, [`autotest.sh`](autotest.sh), orchestrates the agent's workflow:

1. Analyze the current state of tests and code.
2. Use Copilot CLI to generate or improve tests.
3. Run tests and collect results.
4. Identify failures, gaps, or areas for improvement.
5. Iterate: update tests, refactor, and repeat.

Agents are designed to be self-improving, learning from previous iterations and adapting their strategies to maximize coverage and reliability.

## Why?

Automated testing is critical for software quality, but writing and maintaining tests is tedious and error-prone. Autotest aims to:

- Reduce manual effort in test creation and maintenance
- Increase test coverage and reliability
- Enable rapid iteration and feedback
- Explore the limits of autonomous code improvement

## Usage

Run the main agent script:

```bash
./autotest.sh
```

The agent will begin its iterative loop, autonomously improving the test suite. See [`autotest.sh`](autotest.sh) for configuration options.

## Status

Autotest is experimental. Expect rough edges, rapid changes, and lots of learning. Contributions and feedback are welcome!

## License

MIT
