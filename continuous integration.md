# Continuous Integration (CI)

**Continuous integration** is an Agile and DevOps best practice involving the routine integration of code changes into the main branch of a repository, followed by testing these changes as early and as often as possible. Ideally, developers integrate their code daily—if not multiple times a day.

## Benefits of Continuous Integration

Investing in CI leads to **fast feedback** on code changes—sometimes within minutes. This rapid feedback loop contrasts with teams that rely on manual testing, which can take hours or even days to identify issues. By then, new changes may have been introduced, making debugging more complex and time-consuming.

### Protecting Quality with Continuous Builds and Test Automation

How often have we downloaded the latest source code only to find it doesn't compile or is riddled with bugs? CI helps avoid these productivity-killers with two essential practices:

- **Continuous Builds:** Build the project as soon as a change is made, ideally with only a single change-set per build.
- **Test Automation:** Programmatically validate the software to ensure quality. Tests can be initiated from the UI or within the backend services layer.

Think of these two practices as complementary: **Continuous builds** and **test automation** work together in CI to ensure that each build not only completes but also maintains code quality.

> **Note:** To fully realize the benefits of CI, teams must pause development to address any breakages immediately. Building and configuring tests is an investment in quality—keeping builds functional protects that investment.

---

## Testing in CI: Unit, API, and Functional Tests

CI runs typically involve two main phases:
1. **Compilation**: Ensuring that the code compiles.
2. **Testing**: Validating that the code works as intended with automated tests at various levels.

### Types of Tests

1. **Unit Tests**
   - **Purpose**: Validate core components in the code, acting as the first line of defense.
   - **Benefits**: Easy to write, fast, and closely modeled to the code's architecture.
   - **Drawbacks**: Unit tests focus on individual components and may not cover complete user workflows.
   - **Tip**: Reviewing unit tests can help developers understand the expected functionality of specific areas in the codebase.

2. **API Tests**
   - **Purpose**: Test the endpoints between different modules, ensuring they can communicate correctly.
   - **Benefits**: Easy to write, quick to run, and effectively simulate inter-application interactions.
   - **Drawbacks**: In simple code areas, API tests may duplicate some unit tests.
   - **Use Case**: API tests are especially useful for release preparation, providing confidence that interactions between modules are stable before deployment.

3. **Functional Tests**
   - **Purpose**: Model complete user workflows and interactions across the codebase.
   - **Benefits**: More likely to detect bugs by simulating real user actions and testing multiple components together.
   - **Drawbacks**: Slower than unit tests, sometimes prone to false negatives due to network or environmental issues.
   - **Tools**: Tools like HTTPUnit (for fast, basic tests) and Selenium (for comprehensive cross-browser tests) can be used to test user interfaces in web applications.

Functional tests are critical despite their drawbacks, as they can find bugs faster than human testers and free testers to focus on higher-level tasks like **risk analysis**, **test planning**, and even **learning to code**.

---

## Speeding Up CI: Optimizing for Fast Feedback

At Atlassian, we emphasize shortening the developer's feedback loop, ensuring quick builds and test results. Strategies to achieve this include:

- **Parallelizing Tests**: Run tests across multiple servers or "build agents," allowing CI servers to handle numerous tests at once.
- **Scaling with Cloud Resources**: Cloud technologies allow CPU resources to scale based on the test suite size, but avoid redundancy, which can bloat build time and waste resources.
- **Efficient Test Coverage**: Aim for comprehensive test coverage without redundancy. Faster green lights mean faster development.

---

## Branching and CI: A Match Made in Heaven

Many teams avoid branching due to the hassle of merges. However, with modern version control systems like **Git**, branching and merging are simplified. To keep the main code branch ("main" in Git) stable, apply CI processes to all development and stable version branches as well. When builds pass on these branches, teams can confidently merge them into the main branch.

---

## Conclusion: Agile Development at Its Best

Continuous integration, branching, and test automation empower teams to innovate and protect code quality simultaneously. CI enables Agile development at its best by:

- Delivering **working software regularly**
- Minimizing **technical debt**
- Supporting **ongoing innovation**
