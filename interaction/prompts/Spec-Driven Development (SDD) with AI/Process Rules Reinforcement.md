## Process rules reinforcement

**Where the confusion happens**

People often embed **methodology** hints inside the **[Task Text]**, for example:

```md
Write unit tests using AAA.
```

When that happens, it looks like [Triple-A](#triple-a-aaa) lives in the **task**, but architecturally it’s still a **process rule**, not domain content. It’s just being repeated in the **task** for emphasis.

Note: While the Triple A methodology is identified as a standard for high-quality testing, the three “A” terms are not explicitly defined in the prompt, which may reduce clarity for consistent implementation. It is advisable to independently confirm that this interpretation aligns with the specific requirements of your project.

---

### Triple-A (AAA)
<a id="triple-a-aaa"></a>

Triple A (AAA) usually stands for **Arrange, Act, and Assert**.

This pattern organizes a test into three steps:

1. **Arrange** – Prepare inputs, mocks, and initial state.

2. **Act** – Execute the function or behavior being tested.

3. **Assert** – Verify that the outcome matches expectations.
