## 📋 Información del Proyecto

- **Repositorio**: ${{ values.repoName }}
- **Nombre del Microservicio**: ${{ values.projectName }}
- **Departamento**: ${{ values.product }}
- **Tech Lead**: ${{ values.techLead }}

## � Descripción

${{ values.repoDescription }}

Este microservicio está configurado para ejecutarse en Amazon EKS siguiendo los estándares definidos por The Palace Company, con CI/CD automatizado y despliegue mediante Helm charts.

## 🚀 CI/CD y Despliegue

Este repositorio incluye todos los archivos necesarios para:

- **CI/CD automatizado** con GitHub Actions
- **Despliegue en Amazon EKS** mediante Helm
- **Versionado automático** y control de releases
- **Integración completa** con la plataforma de The Palace Company

## 📦 Estructura del Repositorio

```
├── .github/workflows/           # Pipelines CI/CD para build, test y deploy a EKS
├── helm/${{ values.projectName }}/          # Charts de Helm configurados para Amazon EKS
├── version.json                 # Control de versiones automático del microservicio
└── README.md                    # Documentación del proyecto
```

## 🏢 Información del Departamento

Este microservicio pertenece al departamento de **${{ values.product }}** y está bajo la responsabilidad del Tech Lead **${{ values.techLead }}**.

## 🛠️ Desarrollo

Para comenzar a trabajar con este microservicio:

1. Clona el repositorio
2. Revisa la documentación específica del departamento de ${{ values.department }}
3. Contacta al Tech Lead (${{ values.techLead }}) para cualquier duda

## 📚 Recursos Adicionales

- [Documentación de Standards de The Palace Company](https://backstage.thepalace.company)
- [Contactar al Tech Lead: ${{ values.techLead }}](#)
