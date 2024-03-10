Satu behavior yang diperlukan saat menggunakan helm chart ialah menambahkan file config dari satu folder ke-helm chart.

```
  {{- /*
    Glob files to allow them to be mounted by the hub pod

    jupyterhub_config: |
      multi line string content...
    z2jh.py: |
      multi line string content...
  */}}
  {{- (.Files.Glob "files/hub/*").AsConfig | nindent 2 }}
```

Cara ini diambil dari Helm Chart Jupyterhub