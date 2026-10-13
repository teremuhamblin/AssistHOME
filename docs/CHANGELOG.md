# CHANGELOG
>>— OS-Personnel

Toutes les versions majeures du système, de la v1.0.0 à la v5.0.0.

---

## 🟦 v5.0.0 — Quantum Stability Release
### Date
2026-XX-XX

### Ajouts
- Système de mises à jour OTA complet (RAUC)
- Superviseur interne pour gestion des services conteneurisés
- Support multi-plateformes (x86_64, RPi4, RPi5)
- Sécurité renforcée : AppArmor + sandboxing des conteneurs
- Nouveau système de logs centralisé (journald → Loki)

### Modifications
- Optimisation du kernel (réduction de 12% de la taille)
- Docker remplacé par Podman + systemd-nspawn pour services critiques

### Corrections
- Fix ZRAM overflow sur charges lourdes
- Correction du boot UEFI sur certaines cartes mères

---

## 🟦 v4.0.0 — Tactical Expansion Release
### Date
2026-XX-XX

### Ajouts
- Partitionnement dynamique /data (ext4 → btrfs)
- Snapshots système
- Intégration d’un firewall minimal (nftables)
- Support des modules kernel dynamiques

### Modifications
- Amélioration du temps de boot (-18%)
- Réduction de la taille du rootfs SquashFS

### Corrections
- Fix du service Docker au boot
- Correction du mapping réseau sur RPi4

---

## 🟦 v3.0.0 — Operational Services Release
### Date
2026-XX-XX

### Ajouts
- Système de services conteneurisés multi‑instances
- Gestion des secrets (vault minimal)
- Monitoring interne (node-exporter)

### Modifications
- Amélioration de la structure Buildroot
- Optimisation du kernel pour ARM64

### Corrections
- Fix du service SSH sur certaines configurations
- Correction du montage ZRAM

---

## 🟦 v2.0.0 — Structural Enhancement Release
### Date
2026-XX-XX

### Ajouts
- Intégration complète de Docker Engine
- Nouveau layout disque :
  - `/` SquashFS
  - `/data` ext4
  - `/tmp` ZRAM
- Service principal conteneurisé : `core-service`

### Modifications
- Kernel recompilé avec drivers stricts
- Nettoyage du rootfs overlay

### Corrections
- Fix du bootloader U-Boot sur RPi4

---

## 🟦 v1.0.0 — Initial Release
### Date
2026-XX-XX

### Ajouts
- Base Buildroot minimale
- Kernel Linux minimal
- Bootloader U-Boot / GRUB
- SSH activé
- Docker pré‑intégré
- Structure GitHub complète

### Modifications
- N/A

### Corrections
- N/A
