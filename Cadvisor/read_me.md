### 📁 `cadvisor/README.md`

# 🧠 cAdvisor en Kubernetes

Este directorio contiene los manifiestos para desplegar [cAdvisor](https://github.com/google/cadvisor) como un **DaemonSet** en un clúster de Kubernetes.

cAdvisor recolecta métricas a nivel de contenedor: uso de CPU, memoria, disco, y proporciona una interfaz visual por cada nodo.

---

## 📦 Archivos incluidos

- `cadvisor-daemonset.yaml`: Despliegue de cAdvisor
- `cadvisor-service.yaml`: Servicio expuesto vía `NodePort` en el puerto 8080

---
