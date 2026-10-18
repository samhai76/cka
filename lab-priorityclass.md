# Lab: PriorityClass

## Setup

Apply the manifest to create the existing PriorityClasses:

```bash
kubectl apply -f lab-priorityclass.yaml
kubectl get priorityclass
```

## Task

**1.** Create a new `PriorityClass` named **high-priority** intended for user workloads, with a value that is **one less** than the highest existing user-defined PriorityClass value.

**2.** Patch the existing `Deployment` named **busybox-logger** running in the **priority** namespace to use the **high-priority** PriorityClass.
