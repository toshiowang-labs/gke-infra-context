---
type: observation
title: checkout-api is pinned at three replicas with no HorizontalPodAutoscaler
tags: [declared-intent, obtainability, no-hpa]
timestamp: 2026-09-10T14:51:01Z
---

Object: declared-intent-test/Deployment/checkout-api (cluster support-eval-cluster)
Check: no-hpa

checkout-api runs a fixed replicas = 3 and has no HorizontalPodAutoscaler by design.
Its load is synthetic and constant; autoscaling it would only add churn.
