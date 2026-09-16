## Article

[Lyft Moves Streaming Fleet to Apache Flink Kubernetes Operator](https://www.infoq.com/news/2026/09/lyft-flink-k8s-operator/)

Lyft recently migrated hundreds of production Apache Flink streaming jobs off a homegrown Kubernetes operator they built back in 2020, and switched to the open-source Apache Flink Kubernetes Operator instead. The move unlocked things their in-house tool never had, such as safer "last-state" upgrades, in-place autoscaling, and automatic resource tuning. All while cutting down the maintenance burden of hand-rolling their own control plane.

What I found interesting is the trade-off story: building in-house made sense in 2020 when no mature open-source option existed, but maintaining that fork became a growing cost as the ecosystem matured. I also liked that when Lyft hit a bug in the new operator, they filed it upstream and had a fix merged within days which is a pretty good example of how relying on open source can turn into contributing to it, not just consuming it.

