\# Lessons Learned



\## Desired State



One of the biggest concepts I learned during this project was that Kubernetes continuously works to maintain the desired state.



Deleting a Pod does not remove the application. Instead, Kubernetes detects the difference between the current state and the desired state, then automatically creates a replacement Pod.



\---



\## Deployments



Before this project I thought Deployments simply created Pods.



I learned that Deployments actually manage ReplicaSets, and ReplicaSets are responsible for maintaining Pods.



\---



\## Services



Pods are temporary resources whose IP addresses can change.



Services solve this problem by providing a stable endpoint that automatically forwards traffic to healthy Pods.



\---



\## Rolling Updates



Rather than replacing every Pod simultaneously, Kubernetes creates new Pods gradually while removing older ones.



This minimizes downtime and provides a safer deployment strategy.



\---



\## Biggest Takeaway



The most valuable lesson from this project was understanding why each Kubernetes component exists rather than memorizing kubectl commands.



That mindset made Kubernetes much easier to understand.

