```yaml
rbac:
    defaultPolicy: ""
    policy: |-
      g, system:cluster-admins, role:admin
      g, cluster-admins, role:admin
      g, system:authenticated:oauth, role:admin
    scopes: '[groups]'
```

oc adm policy add-role-to-user admin \
  -n snake-game system:serviceaccount:openshift-gitops:openshift-gitops-argocd-application-controller
