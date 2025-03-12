# 🎯 Generador de Preguntas GIFT para Oposiciones

Plataforma web interactiva para la generación automática de preguntas tipo test en formato GIFT, especialmente diseñada para oposiciones y exámenes oficiales en el ámbito legal y militar.

## 🚀 Características Principales

### 📝 Entrada de Contenido
- **Carga de Documentos**:
  - Formatos soportados: PDF, TXT, Markdown
  - Procesamiento automático del contenido
  - Vista previa con opción de expandir/contraer
  - Función de copiado rápido con indicador visual
  - Botón de copiado con retroalimentación

- **Editor de Texto**:
  - Entrada manual de contenido
  - Soporte para formato Markdown
  - Interfaz intuitiva tipo editor
  - Vista previa en tiempo real

### 🤖 Integración con IA
- **Múltiples Proveedores**:
  - Anthropic (Claude 3 Opus, Sonnet)
  - Deepseek (Chat, Coder)
  - Google (Gemini Pro, 1.5, 2.0)
  - xAI (Grok 1, 2)
  - Alibaba (Qwen)
  - OpenAI (GPT-4, 3.5)

- **Configuración Personalizada**:
  - Selección de modelo con agrupación por proveedor
  - Ajuste de temperatura y tokens
  - Control de generación
  - Manejo de errores mejorado
  - Validación de API keys

### 📋 Generación de Preguntas
- **Tipos de Preguntas**:
  - Espacios en blanco (5%)
  - Preguntas textuales (75%)
  - Identificación de incorrectas (10%)
  - "Ninguna es correcta" (10%)

- **Niveles de Dificultad**:
  - Difícil
  - Muy difícil
  - Extremadamente difícil

### 📚 Formato GIFT Mejorado
- **Estructura de Preguntas**:
  - Título y referencia normativa
  - Pregunta principal
  - 4 opciones de respuesta
  - Retroalimentación detallada
  - Validación de formato

- **Retroalimentación Enriquecida**:
  - Fundamento conceptual
  - Relevancia operativa
  - Relaciones clave
  - Aplicación práctica
  - Reglas mnemotécnicas

### 💾 Gestión de Contenido
- **Historial**:
  - Registro de preguntas generadas
  - Marca de tiempo
  - Opción de reutilización
  - Evita duplicados

- **Exportación**:
  - Descarga en formato GIFT
  - Copia al portapapeles con confirmación visual
  - Compatible con Moodle
  - Validación de formato

## 🛠️ Tecnologías Utilizadas

### Frontend
- Next.js 14
- React con Hooks
- TailwindCSS
- TypeScript

### Backend
- Node.js
- Express
- API REST
- Manejo de errores robusto

### Base de Datos
- MongoDB/PostgreSQL (pendiente de implementar)

## 📦 Instalación

1. Clonar el repositorio:
```bash
git clone [URL_DEL_REPOSITORIO]
```

2. Instalar dependencias:
```bash
npm install
```

3. Configurar variables de entorno:
```bash
cp .env.example .env
```

4. Iniciar el servidor de desarrollo:
```bash
npm run dev
```

## 🔑 Configuración de API Keys

Para utilizar los diferentes modelos de IA, necesitas configurar las siguientes API keys:

- OPENAI_API_KEY (GPT-4, 3.5)
- ANTHROPIC_API_KEY (Claude 3)
- GOOGLE_API_KEY (Gemini)
- DEEPSEEK_API_KEY (Chat, Coder)
- XAI_API_KEY (Grok)
- ALIBABA_API_KEY (Qwen)

## 🎯 Público Objetivo

- Opositores y estudiantes
- Educadores y formadores
- Profesionales del ámbito legal/militar
- Creadores de contenido educativo

## 🔄 Flujo de Trabajo

1. **Inicio**: Selección de modo de entrada (archivo/texto)
2. **Configuración**: 
   - Selección de modelo de IA
   - Configuración de tipos de preguntas
   - Ajuste de niveles de dificultad
3. **Procesamiento**: Análisis del contenido
4. **Generación**: Creación de preguntas con validación
5. **Revisión**: Verificación y ajuste
6. **Exportación**: Descarga o copia con confirmación

## 🌟 Características en Desarrollo

- [ ] Integración con LMS
- [ ] Sistema de usuarios
- [ ] Base de datos de preguntas
- [ ] API pública
- [ ] Más formatos de exportación
- [ ] Historial de generación
- [ ] Validación avanzada de formato GIFT

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE.md](LICENSE.md) para más detalles.

## 🤝 Contribuir

Las contribuciones son bienvenidas. Por favor, lee [CONTRIBUTING.md](CONTRIBUTING.md) para detalles sobre nuestro código de conducta y el proceso para enviarnos pull requests.