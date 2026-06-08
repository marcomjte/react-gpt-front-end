# react-gpt-front-end

Frontend de la aplicación **React GPT**, construida con React 18 + TypeScript + Vite. Interfaz de usuario que consume el backend [react-gpt-back-end](https://github.com/marcomjte/react-gpt-back-end) para interactuar con los modelos de OpenAI.

## Características

- Chat con modelos de OpenAI (completions, generación de imágenes, etc.)
- Asistente personalizado vía endpoint `/sam-assistant`
- Renderizado de respuestas en Markdown
- Navegación entre secciones con React Router
- UI responsiva con Tailwind CSS

## Stack tecnológico

- **Framework**: React 18
- **Lenguaje**: TypeScript 5
- **Build tool**: Vite 4
- **Estilos**: Tailwind CSS 3
- **Routing**: React Router DOM v6
- **Markdown**: react-markdown v9

## Requisitos previos

- Node.js 18+
- El backend [react-gpt-back-end](https://github.com/marcomjte/react-gpt-back-end) corriendo localmente

## Instalación

1. Clonar el repositorio:

```bash
git clone https://github.com/marcomjte/react-gpt-front-end.git
cd react-gpt-front-end
```

2. Instalar dependencias:

```bash
npm install
```

3. Crear el archivo de variables de entorno:

```bash
cp .env.template .env
```

4. Verificar que las URLs apunten al backend correcto (por defecto ya están configuradas):

```env
VITE_GPT_API=http://localhost:3000/gpt
VITE_ASSISTANT_API=http://localhost:3000/sam-assistant
```

5. Levantar el servidor de desarrollo:

```bash
npm run dev
```

La app estará disponible en `http://localhost:5173`.

## Scripts disponibles

| Comando | Descripción |
|---|---|
| `npm run dev` | Servidor de desarrollo con HMR |
| `npm run build` | Compilar para producción |
| `npm run preview` | Previsualizar el build de producción |
| `npm run lint` | Linting con ESLint |

## Variables de entorno

| Variable | Descripción |
|---|---|
| `VITE_GPT_API` | URL del endpoint GPT del backend |
| `VITE_ASSISTANT_API` | URL del endpoint del asistente personalizado |

## Proyecto relacionado

Este frontend trabaja en conjunto con el backend:
→ [react-gpt-back-end](https://github.com/marcomjte/react-gpt-back-end) — NestJS + OpenAI API

## Licencia

MIT
