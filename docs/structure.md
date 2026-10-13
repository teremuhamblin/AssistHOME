###### structure.md >> markdown
# ✅ Structure du Projet
>>— OS-Personnel

```text
os-personnel/
│
├── README.md
├── structure.md
├── architecture.md
├── version.md
├── maintainers.md
├── all-contributors.md
│
├── buildroot/
│   ├── configs/
│   ├── board/
│   └── overlay/
│
├── core-service/
│   └── Dockerfile
│
└── .github/
    ├── CONTRIBUTING.md
    ├── SECURITY.md
    ├── CODEOFCONDUCT.md
    ├── SUPPORT.md
    └── CODEOWNERS
```

### 📌 Description rapide
- **buildroot/** : configuration du système d’exploitation.
- **core-service/** : conteneur principal lancé au boot.
- **.github/** : gouvernance du projet.

---
