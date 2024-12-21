# Take Practice Test Activity Diagram

```mermaid
stateDiagram-v2
    [*] --> Login
    Login --> SelectTest
    SelectTest --> ViewInstructions
    ViewInstructions --> StartTest
    StartTest --> AnswerQuestions
    AnswerQuestions --> SubmitTest
    SubmitTest --> CalculateScore
    CalculateScore --> DisplayResults
    DisplayResults --> ViewProgress
    ViewProgress --> [*]
```