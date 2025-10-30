## 📋 Información del Proyecto

- **Repositorio**: ${{ values.repoName }}
- **Nombre de la función**: ${{ values.projectName }}
- **Mercado**: ${{ values.market }}
- **Producto**: ${{ values.product }}
- **Tech Lead**: ${{ values.techLead }}

## ⚙️ Descripción

${{ values.repoDescription }}

Esta función serverless está configurada para ejecutarse en AWS Lambda siguiendo los estándares definidos por The Palace Company, con CI/CD automatizado y despliegue mediante Serverless Framework.

## 🚀 CI/CD y Despliegue

Este repositorio incluye todos los archivos necesarios para:

- **CI/CD automatizado** con GitHub Actions
- **Despliegue en AWS Lambda** mediante Serverless Framework
- **Versionado automático** y control de releases
- **Integración completa** con la plataforma de The Palace Company
- **Auto-scaling** automático basado en demanda

## 📦 Estructura del Repositorio

```
├── .github/workflows/           # Pipelines CI/CD para build, test y deploy a AWS Lambda
├── version.json               # Control de versiones automático de la función
└── README.md                  # Documentación del proyecto
```

## 🏢 Información Organizacional

Esta función serverless pertenece al mercado de **${{ values.market }}**, producto **${{ values.product }}** y está bajo la responsabilidad del Tech Lead **${{ values.techLead }}**.

## 🛠️ Desarrollo Local

Para comenzar a trabajar con esta función serverless:

1. **Clona el repositorio**

   ```bash
   git clone https://github.com/the-palace-company/${{ values.repoName }}.git
   cd ${{ values.repoName }}
   ```

2. **Prerequisitos**

   - Node.js 18+
   - Serverless Framework CLI
   - AWS CLI configurado

3. **Desarrollo local**

   ```bash
   npm install
   serverless offline start
   ```

4. **Deploy manual (QA)**

   ```bash
   serverless deploy --stage qa
   ```

5. **Contacta al Tech Lead (${{ values.techLead }}) para cualquier duda**

## ⚡ Configuración AWS Lambda

- **Runtime**: Node.js 18.x
- **Región**: us-east-1
- **Función**: `${{ values.market | lower }}-${{ values.product | lower }}-${{ values.projectName | lower }}`
- **API Gateway**: Configurado automáticamente
- **Auto-scaling**: Configuración automática basada en demanda
- **Monitoring**: Integrado con CloudWatch y Datadog

## 📚 Recursos Adicionales

- [Documentación de Standards de The Palace Company](https://backstage.thepalace.company)
- [Contactar al Tech Lead: ${{ values.techLead }}](#)
