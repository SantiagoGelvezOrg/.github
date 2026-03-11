# santiagogelvez-dev

Ecosistema de aplicaciones web, SaaS y proyectos personales bajo [santiagogelvez.com](https://santiagogelvez.com).

## 🌐 Portafolio
- **portfolio** — [santiagogelvez.com](https://santiagogelvez.com)

## 🎨 Frontend Mentor
- **frontendmentor-gallery** — Galería de retos completados
- Retos individuales: filtrá por topic `frontendmentor`

## 💼 SaaS
| App | Subdominio |
|-----|------------|
| hr-platform | hr.santiagogelvez.com |
| clirap | clirap.santiagogelvez.com |
| inventario-app | inventario.santiagogelvez.com |
| turnos-app | turnos.santiagogelvez.com |
| factura-app | factura.santiagogelvez.com |
| agencia-app | agencia.santiagogelvez.com |
| aula-app | aula.santiagogelvez.com |

## 📊 Proyectos personales
- **dash-colombia** — Dashboards de datos abiertos de Colombia
- **mundial-2026** — Tracker interactivo del Mundial 2026
- **finance-app** — Finanzas personales

## 🛠️ Stack principal
React · Next.js · Vue 3 · NestJS · FastAPI · Go · PostgreSQL · Redis · AWS · Cloudflare · Terraform
```

### 2. Crear repo `infra`

1. Creá un nuevo repo llamado **`infra`**
2. Visibilidad: **Private**
3. Inicializá con un README básico

Luego subí el código Terraform que ya tenés (el módulo `s3-subdomain`). Estructura sugerida:
```
infra/
├── modules/
│   └── s3-subdomain/        ← el módulo que ya tenés
├── envs/
│   └── prod/
│       ├── main.tf           ← donde invocás los módulos
│       ├── variables.tf
│       └── terraform.tfvars  ← en .gitignore (tiene el token de Cloudflare)
├── .gitignore
└── README.md
```

**Importante:** el `.gitignore` debe incluir:
```
*.tfvars
*.tfstate
*.tfstate.backup
.terraform/
