### 📁 `grafana/README.md`

# 📈 Grafana en Kubernetes

Este directorio contiene los archivos necesarios para desplegar [Grafana](https://grafana.com/) en un clúster Kubernetes.

Grafana permite la visualización de métricas desde Prometheus, Node Exporter, cAdvisor y otras fuentes.

---

## 📦 Archivos incluidos

- `grafana-deployment.yaml`: Despliegue de Grafana en el namespace `monitoring`
- `grafana-service.yaml`: Servicio expuesto vía `NodePort` en el puerto 3000

---
