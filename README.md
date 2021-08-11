# Fluent bit kubernetes logging 

Ship and parser kubernetes logs to external Elastic.

### Installation

```
kubectl create namespace logging
kubectl apply -f https://raw.githubusercontent.com/thangtq710/fluent-bit-kubernetes-logging/master/files/1-fluent-bit-service-account.yaml
kubectl apply -f https://raw.githubusercontent.com/thangtq710/fluent-bit-kubernetes-logging/master/files/2-fluent-bit-role.yaml
kubectl apply -f https://raw.githubusercontent.com/thangtq710/fluent-bit-kubernetes-logging/master/files/3-fluent-bit-role-binding.yaml
kubectl apply -f https://raw.githubusercontent.com/thangtq710/fluent-bit-kubernetes-logging/master/files/4-fluent-bit-configmap.yaml
kubectl apply -f https://raw.githubusercontent.com/thangtq710/fluent-bit-kubernetes-logging/master/files/5-fluent-bit-ds.yaml
```

### Reference

- https://docs.fluentbit.io/manual/installation/kubernetes
- https://github.com/fluent/fluent-bit/issues/1450
- https://docs.nginx.com/nginx/admin-guide/monitoring/logging/