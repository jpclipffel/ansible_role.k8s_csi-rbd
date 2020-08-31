# Ansible role - `k8s_csi-rbd`

Manage Ceph's RBD CSI plugin on Kubernetes clusters.

## Tags

| Tag      | Description                      |
|----------|----------------------------------|
| `apply`  | Deploy Ceph's RBD plugin for CSI |
| `delete` | Delete Ceph's RBD plugin for CSI |
 
## Variables

| Variable                 | Type     | Required | Defaut                              | Description           |
|--------------------------|----------|----------|-------------------------------------|-----------------------|
| `k8s_csi_rbd_repository` | `string` | No       | "https://ceph.github.io/csi-charts" | Helm chart repository |
| `k8s_csi_rbd_chart`      | `string` | No       | "ceph-csi-rbd"                      | Helm chart name       |
| `k8s_csi_rbd_release`    | `string` | No       | "ceph-csi-rbd"                      | Helm release name     |
| `k8s_csi_rbd_namespace`  | `string` | No       | "kube-system"                       | Namepsace to use      |


## Tasks sequence

```text
--------------------------- tags: apply, delete --
main.yml
```
