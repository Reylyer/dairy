`systemd` merupakan [[init]] system yang digunakan mayoritas distribusi linux sekarang, period. `systemd` 

## Basic Usage

Penggunaan systemd yang umum digunakan antara lain `status`, `enable`, dan `start`. Kita

### Melihat status service

```
# systemctl status NetworkManager.service
```

### Menjalakan service saat boot

```
# systemctl enable NetworkManager.service
```

### Memulai service sekarang (non-persistent)

```
# systemctl start NetworkManager.service
```

## Membuat Unit File

-- WIP