# miprimerproyecto

Gestor de Entregas con Google Maps - Aplicación web para gestionar entregas de paquetes utilizando Google Maps.

## 🚀 Características

- Interfaz intuitiva para gestionar entregas
- Integración con Google Maps
- Diseño responsive
- Despliegue automatizado en Vercel

## 📋 Requisitos Previos

- Git
- Cuenta en Vercel (https://vercel.com)
- Google Maps API Key

## 🔧 Instalación Local

1. Clona el repositorio:
```bash
git clone <tu-repositorio>
cd miprimerproyecto
```

2. Instala las dependencias:
```bash
npm install
```

3. Configura tu API Key de Google Maps:
   - Copia el archivo `.env.local.example` a `.env.local`
   - Reemplaza `YOUR_API_KEY_HERE` con tu clave de API de Google Maps
   - También actualiza la clave en `index.html`

4. Inicia el servidor de desarrollo:
```bash
npm run dev
```

## 🌐 Despliegue en Vercel

### Opción 1: Desde la Terminal (Recomendado)

1. Instala Vercel CLI:
```bash
npm i -g vercel
```

2. Inicia el despliegue:
```bash
vercel
```

3. Sigue las instrucciones interactivas

### Opción 2: Conectar Repositorio GitHub

1. Haz push de tu código a GitHub
2. Ve a https://vercel.com
3. Haz clic en "New Project"
4. Selecciona tu repositorio
5. Vercel detectará automáticamente la configuración
6. Haz clic en "Deploy"

## 🔐 Variables de Entorno en Vercel

Después de desplegar:

1. Ve a tu proyecto en Vercel
2. Abre "Settings" → "Environment Variables"
3. Agrega una nueva variable:
   - **Name**: `GOOGLE_MAPS_API_KEY`
   - **Value**: Tu API Key de Google Maps
4. Redeploy el proyecto

## 📝 Notas Importantes

- **Google Maps API Key**: Asegúrate de tener habilitadas las APIs correctas en Google Cloud Console
- **Seguridad**: Nunca hagas commit de tu `.env.local` (ya está en `.gitignore`)
- **Dominio personalizado**: Puedes conectar un dominio personalizado en Vercel

## 📦 Estructura del Proyecto

```
miprimerproyecto/
├── index.html           # Página principal
├── package.json         # Configuración de npm
├── vercel.json          # Configuración de Vercel
├── .env.local           # Variables de entorno (local)
├── .gitignore           # Archivos ignorados por git
└── README.md            # Este archivo
```

## ✅ Checklist de Despliegue

- [ ] Verificar que `index.html` está en la raíz del proyecto
- [ ] Reemplazar `YOUR_API_KEY_HERE` con tu Google Maps API Key
- [ ] Configurar variables de entorno en Vercel
- [ ] Hacer push del código a GitHub
- [ ] Configurar el proyecto en Vercel
- [ ] Verificar que la aplicación funciona correctamente

## 🆘 Solución de Problemas

**Problema**: "API Key not valid"
- Solución: Verifica que tu API Key está correctamente configurada en Google Cloud Console

**Problema**: CORS errors
- Solución: Asegúrate de que tu dominio de Vercel está autorizado en Google Cloud

**Problema**: Mapa no se carga
- Solución: Comprueba que JavaScript está habilitado en tu navegador

## 📧 Soporte

Para más información sobre Vercel, visita: https://vercel.com/docs 
