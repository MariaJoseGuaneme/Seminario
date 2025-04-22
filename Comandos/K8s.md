### Ver todos los recursos en un namespace
```bash
kubectl get all -n <namespace>
```

### Ver todos los pods en un namespace
```bash
kubectl get pods -n <namespace>
```

### Ver todos los deployments en un namespace
```bash
kubectl get deployments -n <namespace>
```

### Ver todos los servicios en un namespace
```bash
kubectl get services -n <namespace>
```

### Ver todos los ConfigMaps en un namespace
```bash
kubectl get configmaps -n <namespace>
```

### Ver detalles de un recurso específico
```bash
kubectl describe <recurso> <nombre> -n <namespace>
```

### Acceder a la terminal de un contenedor dentro de un pod
```bash
kubectl exec -it <nombre-del-pod> -n <namespace> -- /bin/bash
# O usar /bin/sh si bash no está instalado
kubectl exec -it <nombre-del-pod> -n <namespace> -- /bin/sh
```

### Crear/actualizar un ConfigMap usando un archivo local
```bash
kubectl create configmap <nombre-del-configmap> \
  --from-file=nginx.conf=<ruta-del-archivo> \
  -n <namespace> --dry-run=client -o yaml | kubectl apply -f -
```

### Ejemplo con Prometheus
```bash
kubectl create configmap prometheus-config \
  --from-file=prometheus.yml=/home/majog/prometheus.yml \
  -n monitoring --dry-run=client -o yaml | kubectl apply -f -
```

### Reiniciar un deployment (útil tras actualizar un ConfigMap o imagen)
```bash
kubectl rollout restart deployment <nombre-del-deployment> -n <namespace>
```

### Ejemplo con Prometheus
```bash
kubectl rollout restart deployment prometheus -n monitoring
```

### Eliminar un servicio del clúster
```bash
kubectl delete service <nombre-del-servicio> -n <namespace>
```

### Ejemplo
```bash
kubectl delete service nginx-exporter -n default
```
