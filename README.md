# nmagro-r-iot-argocd

Repo público que vigila Argo CD en la Parte 3 de Inception-of-Things (42).

- `k8s/deployment.yaml`: la app de Wil (`wil42/playground`, puerto 8888) en el namespace `dev`.
- `k8s/service.yaml`: la expone en el puerto 8888.

Para pasar de v1 a v2 se cambia la tag de la imagen en `k8s/deployment.yaml` y se hace push. Argo CD lo detecta y actualiza la app.
