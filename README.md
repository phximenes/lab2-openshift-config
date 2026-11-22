# lab2-openshift-config

Material de partida (Kustomize) do **Laboratório Final 2 de Red Hat OpenShift** (curso 200DEV).

Estrutura:

- `base/`: Deployment, Service e Route da aplicação, sem dados de ambiente.
- `overlays/dev/` e `overlays/prod/`: `kustomization.yaml` que apontam para a base e definem a imagem de cada ambiente.

Antes de usar, substitua `<REGISTRY>` e `<usuario>` nos arquivos `kustomization.yaml` pelos valores indicados no enunciado do laboratório.

Validação local:

```
kubectl kustomize overlays/dev
kubectl kustomize overlays/prod
```
