###### architecture.md >> markdown
# Architecture
>>— OS-Personnel
   - v1.0.0

## 🧱 Couches principales
### 1. Bootloader
- U-Boot (ARM) ou GRUB (x86_64)

### 2. Kernel Linux
- Config minimaliste
- Drivers strictement nécessaires

### 3. Base OS (Buildroot)
- Busybox
- Systemd ou init simple
- SSH activé

### 4. Conteneurs
- Docker Engine
- Service principal : `core-service`

### 5. Système de fichiers
- `/` : SquashFS (lecture seule)
- `/data` : ext4 (persistant)
- `/tmp` : ZRAM

### 🔄 Cycle de boot
1. Bootloader → Kernel  
2. Kernel → Init  
3. Init → Docker  
4. Docker → core-service
