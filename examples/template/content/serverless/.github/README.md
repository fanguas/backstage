## 📋 Información del Proyecto

- **Repositorio**: ${{ values.repoName }}
- **Nombre del microservicio**: ${{ values.projectName }}
- **Mercado**: ${{ values.market }}
- **Producto**: ${{ values.product }}
- **Tech Lead**: ${{ values.techLead }}

## ⚙️ Descripción

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
│   ├── Chart.yaml              # Metadatos del chart de Helm
│   └── values/                 # Configuraciones por ambiente
│       └── qa.yaml            # Configuración específica para QA
├── version.json              # Control de versiones automático del microservicio
└── README.md                 # Documentación del proyecto
```

## 🏢 Información Organizacional

Este microservicio pertenece al mercado de **${{ values.market }}**, producto **${{ values.product }}** y está bajo la responsabilidad del Tech Lead **${{ values.techLead }}**.

## 🛠️ Desarrollo Local

Para comenzar a trabajar con este microservicio:

1. **Clona el repositorio**

   ```bash
   git clone https://github.com/the-palace-company/${{ values.repoName }}.git
   cd ${{ values.repoName }}
   ```

2. **Prerequisitos**

   - Docker
   - kubectl configurado
   - Helm 3.x

3. **Deploy manual con Helm (QA)**

   ```bash
   helm install ${{ values.projectName | lower }} ./helm/${{ values.projectName }}/ \
     --values ./helm/${{ values.projectName }}/values/qa.yaml \
     --namespace ${{ values.market | lower }}-${{ values.product | lower }} \
     --create-namespace
   ```

4. **Contacta al Tech Lead (${{ values.techLead }}) para cualquier duda**

## ☸️ Configuración EKS

- **Cluster**: `tpc-${{ values.market | lower }}-eks-cluster`
- **Namespace**: `${{ values.market | lower }}-${{ values.product | lower }}`
- **Service**: `${{ values.projectName | lower }}-service`
- **Istio**: Configurado automáticamente con service mesh
- **HPA**: Auto scaling configurado (min: 2, max: 10 pods)
- **Monitoring**: Integrado con Datadog

## 📚 Recursos Adicionales

- [Documentación de Standards de The Palace Company](https://backstage.thepalace.company)
- [Contactar al Tech Lead: ${{ values.techLead }}](#)
