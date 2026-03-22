# Immozy — Site web de présentation

Site vitrine de l'application mobile **Immozy** — gestion locative simplifiée.

## Structure

```
immozy-website/
├── index.html          # Page principale (tout-en-un, assets embarqués)
└── .github/
    └── workflows/
        └── deploy.yml  # CI/CD : déploiement automatique sur OVH via FTP
```

## Déploiement automatique

Tout push sur la branche `master` déclenche automatiquement le déploiement sur OVH.

### Secrets GitHub requis

Configurer dans **Settings → Secrets and variables → Actions** :

| Secret | Valeur |
|--------|--------|
| `FTP_SERVER` | `ftp.cluster129.hosting.ovh.net` |
| `FTP_USERNAME` | Ton identifiant FTP OVH |
| `FTP_PASSWORD` | Ton mot de passe FTP OVH |

## Développement local

Ouvrir `index.html` directement dans un navigateur.
