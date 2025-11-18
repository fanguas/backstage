# Golden Path - The Palace Company

Este repositorio fue generado automáticamente por el Backstage Template (Golden Path).

## 📋 Información del Repositorio

- **Repositorio**: ${{ values.repoName }}
- **Nombre del proyecto**: ${{ values.projectName }}
- **Mercado**: ${{ values.market }}
- **Producto**: ${{ values.product }}
- **Tech Lead**: ${{ values.techLead }}
- **Tipo de arquitectura**: ${{ values.repoType }}

## ⚙️ Descripción

${{ values.repoDescription }}

## 🚀 ¿Qué incluye?

- Estructura base y archivos iniciales según el tipo de arquitectura seleccionado (Vue, Serverless, ECS, EKS)
- CI/CD automatizado con GitHub Actions
- Configuración para despliegue en la plataforma correspondiente
- Versionado automático y control de releases
- Permisos asignados automáticamente al equipo de GitHub según el producto
- Registro en el catálogo de Backstage
- Ticket de infraestructura creado en Jira

## 📦 Estructura del Repositorio

```
├── .github/workflows/           # Pipelines CI/CD
├── src/                        # Código fuente del proyecto
├── version.json                # Control de versiones automático
└── README.md                   # Documentación del proyecto
```

## 🏢 Información Organizacional

Este proyecto pertenece al mercado de **${{ values.market }}**, producto **${{ values.product }}** y está bajo la responsabilidad del Tech Lead **${{ values.techLead }}**.

## 🛠️ Primeros Pasos

1. **Clona el repositorio**

   ```bash
   git clone https://github.com/the-palace-company/${{ values.repoName }}.git
   cd ${{ values.repoName }}
   ```

2. **Revisa la documentación y estructura generada**

3. **Contacta al Tech Lead (${{ values.techLead }}) para dudas o soporte**

## 📚 Recursos Adicionales

- [Documentación de Standards de The Palace Company](https://backstage.thepalace.company)
- [Contactar al Tech Lead: ${{ values.techLead }}](#)
