{{- define "containerinfo.clusterrole" -}}
{{- if .Values.deployment.serviceAccount.create -}}
apiVersion: rbac.authorization.k8s.io/v1
kind: ClusterRole
metadata:
  name: {{ include "containerinfo.name" . }}
rules:
- apiGroups: [""]
  resources: ["pods", "namespaces"]
  verbs: ["get", "list", "watch"]
{{- end }}
{{- end }}