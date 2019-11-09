---
title: Kubernetes Scale
date: 2019-02-02
tags: ["kubernetes", "scale"]
---

Learn to scale kubernetes deployments

<!--more-->

```sh
    $ kubectl scale --replicas=<expected_replica_num> deployment <deployment_name># kubectl scale --replicas=4 deployment my-nginxdeployment "my-nginx" scaled
```

Now, check whether it is running:
```sh
    $ kubectl get pods
    NAME                                   READY     STATUS    RESTARTS   AGE
    kubernetes-bootcamp-5c69669756-wv2rp   1/1       Running   0          11s
```

We can check application logs:
```sh
$ kubectl logs kubernetes-bootcamp-5c69669756-wv2rp
Kubernetes Bootcamp App Started At: 2018-10-20T13:38:41.537Z | Running On:  kubernetes-bootcamp-5c69669756-wv2rp
```

This change is pushed from Travis-CI.
