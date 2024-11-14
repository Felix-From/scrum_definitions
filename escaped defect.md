# Escaped Defects

## What Are Escaped Defects?

Escaped defects refer to the number of issues or bugs found in a software product **after it has been released into production**, which were not detected during the pre-release testing phases. This metric is calculated by counting all the defects reported by users of the product after its release. Essentially, it measures the defects that have 'escaped' the earlier stages of quality assurance and testing, reaching the end-user.

The **lower the number of escaped defects**, the more effective a team's testing processes are considered to be.

---

## Why Are Escaped Defects Important?

### 1. **Quality Assurance**
Escaped defects are a direct indicator of the quality of the testing and quality assurance processes within a software development team. By monitoring this metric, teams can gauge how effective their testing strategies are at catching bugs before software products are released. This is crucial for maintaining high standards of quality and ensuring that end-users have a smooth and functional experience with the product.

### 2. **Customer Satisfaction**
High numbers of escaped defects can lead to **user frustration** and decreased trust in the software product and the brand. By keeping escaped defects to a minimum, companies can enhance user satisfaction and loyalty. It is much more costly both in terms of support resources and brand reputation to fix issues after release rather than catching them earlier in the testing phase.

### 3. **Cost Efficiency**
Addressing defects after a product has been released is often more costly than fixing issues during development. Post-release fixes require **hotfixes, patches**, and sometimes even full version updates, which can be resource-intensive. Monitoring escaped defects helps in reducing these costs by increasing the efficiency of the testing process, thereby catching more errors before they make it to the live environment.

---

## Limitations of Escaped Defects

### 1. **Does Not Measure Severity**
Escaped defects as a metric does not distinguish between the severity of the defects. A high count of escaped defects might be misleading if many of these issues are minor and do not significantly impact the user experience, whereas even a single critical defect escaping could be disastrous.

### 2. **Not a Standalone Metric**
Relying solely on escaped defects to assess the quality of a software product can be misleading. This metric should be used in conjunction with other quality and performance metrics to provide a **comprehensive view** of the software's health and the effectiveness of the development process.

### 3. **Lacks Context on Cause**
While this metric tracks the number of defects that have escaped into production, it does not provide insights into **why** these defects were not caught. Without understanding the underlying reasons—be it insufficient test coverage, rushed releases, or inadequate test cases—simply knowing the number of escaped defects offers limited actionable intelligence.

---

## Metrics Related to Escaped Defects

### 1. **Defect Density**
Defect density helps to provide context to the escaped defects metric by measuring the number of defects relative to the size of the software (typically per thousand lines of code). This metric is crucial for understanding whether a high number of escaped defects is due to a larger codebase or poor quality assurance practices.

### 2. **Test Pass Rate**
The test pass rate measures the percentage of tests that pass successfully as part of the testing phase. A high test pass rate typically suggests fewer defects. However, if the escaped defects number is also high despite a high test pass rate, it might indicate insufficient test coverage or ineffective test cases.

### 3. **Change Failure Rate**
Change failure rate measures how often changes or updates to the software lead to failures in production. A high change failure rate in conjunction with a high number of escaped defects can indicate **systemic issues** in both the development and the deployment processes, highlighting areas that may need strategic improvements.
