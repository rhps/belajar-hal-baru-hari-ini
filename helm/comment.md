Saat bekerja dengan helm, kadang kita butuh untuk men-non-aktif-kan suatu bagian dari kode. Berikut ada caranya

```
      {{- /* # disable tolerations
      
      {{- with concat .Values.scheduling.corePods.tolerations .Values.hub.tolerations }}
      tolerations:
        {{- . | toYaml | nindent 8 }}
      {{- end }}
      
      */}}
```

Multiline comment di-helm chart dibuka dengan `{{- /*` dan diakhri dengan `*/}}`