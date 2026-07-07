rbac:
    defaultPolicy: ""
    policy: |-
      g, system:cluster-admins, role:admin
      g, cluster-admins, role:admin
      g, system:authenticated:oauth, role:admin
    scopes: '[groups]'
