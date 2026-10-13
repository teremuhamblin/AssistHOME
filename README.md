###### README.md >> markdown 

---

# 📦 AssistHOME

## ✅ OS-Personnel
   - — Version 5.0.0
   - — Quantum Stability Release

**Système d’exploitation sécurisé et conteneurisé, conçu pour une mission unique** :  
```text
Fournir une base stable, résiliente et auto‑maintenue pour exécuter un service principal ou un ensemble de services en environnement contrôlé.
```

---

### 🎯 Objectifs
>> v5.0.0
```text
- OS minimal basé sur Buildroot
- Rootfs en lecture seule (SquashFS) pour garantir l’intégrité
- Partition /data en btrfs avec snapshots (v4+)
- Podman comme moteur de conteneurs (Docker toujours supporté)
- Superviseur interne (v5+) pour orchestrer les services
- Mises à jour OTA via RAUC (v5+)
- Sécurité avancée : AppArmor, sandboxing, firewall nftables
- Multi‑plateformes : x86_64 UEFI, Raspberry Pi 4, Raspberry Pi 5
- Architecture modulaire, évolutive, doctrinale
```

### 🧬 Capacités principales
>> v1 → v5
```text
- v1 : Fondation Buildroot + Docker + SquashFS  
- v2 : Renforcement structurel + ZRAM + optimisation kernel  
- v3 : Multi‑services + monitoring + gestion des secrets  
- v4 : Migration ext4 → btrfs + snapshots + firewall + modules dynamiques  
- v5 : OTA RAUC + superviseur interne + AppArmor + multi‑plateformes + logs centralisés
```

### 📁 Structure
> Voir **structure.md** pour l’organisation complète du projet.

### 🧩 Architecture
> Voir **architecture.md** pour les couches techniques et le cycle de boot.

---

### 🛠️ Buildroot & Système
```text
- Configurations multi‑plateformes (configs/)
- Kernel minimal optimisé (linux.config)
- Overlay strict (overlay/)
- Services systemd (docker.service, core-service.service, supervisor.service)
- Scripts d’initialisation (os-init.sh)
- Packages internes (Docker, Podman, Supervisor)
```

### 🔧 Mainteneurs
> Voir **maintainers.md**

---

### 👥 Contributeurs
> Voir **all-contributors.md**

---

### 📅 Roadmap & Versions
- Roadmap complète v1 → v5 : ROADMAP.md
- Historique complet : CHANGELOG.md
- Milestones : milestone.md
- Releases globales : release.md

---

### 🔐 Sécurité
> Voir **.github/SECURITY.md**

- Inclut :
   - AppArmor (v5)
   - nftables firewall (v4+)
   - Rootfs en lecture seule
   - Sandboxing des conteneurs
   - Gestion des secrets (v3+)

### 🛡️ Résilience & Maintenance
- Snapshots btrfs (v4+)
- Mises à jour OTA RAUC (v5)
- Superviseur interne (v5)
- Logs centralisés via Loki (v5)

### 📜 Licence
>LICENSE AssistHOME PERSO  
- Libre d’utilisation et de modification.

---

### 🧭 Gouvernance GitHub
- Issues globales : issue.md
- Discussions globales : discussion.md
- PR globales : pull_request.md
- Support : .github/SUPPORT.md
- Code de conduite : .github/CODEOFCONDUCT.md
- Contributing : .github/CONTRIBUTING.md

---

### 🧱 État du projet
OS-Personnel v5.0.0 est désormais un système complet, stable, sécurisé, auto‑maintenu et multi‑plateformes, prêt pour les évolutions v6+ (HA‑like, cluster, nodes, etc.).
