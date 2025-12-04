# Step Runner

The `Step Runner` component is the one in charge of configuring and starting the process once the scene loads.

The training process will be configured by adding and nesting steps to the `Execution Steps` field:

![execution-runner-step-list.png](../../../.attachments/execution-runner-step-list.png)

![process-hierarchy-example.png](./.attachments/process-hierarchy-example.png)

## Process lifecycle

The Step Runner will run each step in a sequential order. If the step is a [StepGroup](../Components/StepGroup.md) or a [ProcessStep](../Components/ProcessStep.md) all of its child steps will be executed before marking it as `Completed`. In this way you can nest single steps and group steps to adequate to each process needs.

The process lifecycle will look like the following diagram:

```mermaid
flowchart TB
id1([Start process execution])-->id6[Initialize]
id6-->id2{Are all steps finished?}
id2---->|Yes|id5([End])
id2---->|No|id3[Run next pending step]
id3---->|Result|id4[Handle result]
id4-->id2
```
