Command `find` di-Linux sangat berguna, karena dapat mencari file/folder dengan kriteria tertentu dengan kemudian dapat melakukan suatu perintah linux lain dari file/folder yang ditemukan tersebut. Sebagai contoh berikut,

```
find "${d}" \
    ! \( \
        -group "${NB_GID}" \
        -a -perm -g+rwX \
    \) \
    -exec chgrp "${NB_GID}" {} \; \
    -exec chmod g+rwx {} \;
```

Command tersebut akan mencari semua file/folder dengan kriteria `ownernya nya bukan di-group tertentu ("${NB_GID}") dan permissionnya bukan group read-write-noexec (-g+rwX)`. Kemudian file/folder tersebut akan dilakukan eksekusi `chgrp` dan `chmod`.