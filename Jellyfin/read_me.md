# 📺 Jellyfin en Kubernetes

Este repositorio contiene los archivos de configuración necesarios para desplegar **Jellyfin**, un servidor multimedia de código abierto, en un clúster de **Kubernetes**.

---

## 🧾 Descripción

[Jellyfin](https://jellyfin.org/) es un sistema de medios gratuito que te permite organizar, administrar y compartir tu biblioteca de películas, series, música y más. Este proyecto lo ejecuta en un entorno contenerizado utilizando Kubernetes.

---

## 📦 Características

- Despliegue de Jellyfin en Kubernetes
- Uso de volúmenes persistentes para almacenar medios
- Exposición del servicio mediante `NodePort` o `Ingress`
- Integración opcional con Prometheus + Grafana para monitoreo (vía `jellyfin-exporter`)
- Preparado para integrarse con un entorno de red con VLANs y bridge

---
