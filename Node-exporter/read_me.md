# 🐧 Node Exporter en Kubernetes

Este directorio contiene los manifiestos necesarios para desplegar [Prometheus Node Exporter](https://github.com/prometheus/node_exporter) como un **DaemonSet** en Kubernetes.

Node Exporter expone métricas del sistema operativo de cada nodo: CPU, memoria, red, almacenamiento, etc.

---

## 📦 Archivos incluidos

- `node-exporter-daemonset.yaml`: Despliega un DaemonSet en el namespace `monitoring`
- `node-exporter-service.yaml`: Crea un servicio `NodePort` en el puerto 9100

---
