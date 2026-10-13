# ROADMAP
>>— OS-Personnel

Plan d’évolution du système de la version 1 à la version 5.

---

## 🟦 v1 — Foundation Layer
### Objectifs
- Construire la base Buildroot
- Intégrer Docker
- Rootfs en SquashFS
- Partition /data persistante
- Service principal conteneurisé

### Livrables
- Image bootable
- Structure GitHub complète
- Documentation initiale

---

## 🟦 v2 — Structural Reinforcement
### Objectifs
- Stabiliser le système
- Améliorer le kernel
- Optimiser le layout disque
- Ajouter ZRAM
- Finaliser le conteneur `core-service`

### Livrables
- OS stable pour usage quotidien
- Documentation architecture v2

---

## 🟦 v3 — Service Expansion
### Objectifs
- Support multi‑services conteneurisés
- Monitoring interne
- Gestion des secrets
- Amélioration ARM64

### Livrables
- Système capable d’héberger plusieurs services
- Dashboard minimal de monitoring

---

## 🟦 v4 — Tactical Features
### Objectifs
- Migration ext4 → btrfs
- Snapshots système
- Firewall intégré
- Modules kernel dynamiques

### Livrables
- OS résilient, orienté production
- Sécurité renforcée

---

## 🟦 v5 — Quantum Stability
### Objectifs
- Mises à jour OTA (RAUC)
- Superviseur interne
- Multi‑plateformes (x86_64, RPi4, RPi5)
- Sécurité avancée (AppArmor)

### Livrables
- OS complet, auto‑maintenu
- Base prête pour versions 6+ (HA‑like)
