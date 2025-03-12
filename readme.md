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

**🟢 Contexto:**
Se requiere desarrollar una plataforma web interactiva que permita a los usuarios adjuntar cualquier documento en formato pdf, txt o docx. y tambien que pueda el usuario escribir texto y comunicarse con la ia para darle instrucciones
La plataforma analizará el contenido del documento utilizando la inteligencia artificial


La tarea principal es diseñar preguntas de opción múltiple en formato GIFT para ser importadas a Moodle. Estas preguntas deben basarse exclusivamente en el contenido del documento proporcionado, sin añadir información externa. Además, cada pregunta debe funcionar como herramienta de estudio: evaluando conocimientos y ofreciendo una retroalimentación detallada que ayude a los estudiantes a comprender los conceptos clave y a memorizar la información para el examen.

**🔵 Rol:**
Eres un experto en desarrollo de aplicaciones web con integración de inteligencia artificial y en la creación de preguntas de opción múltiple para plataformas educativas (especialmente Moodle), con más de 20 años de experiencia en ambos campos.

Dominas tanto la programación web (Frontend y Backend) como la integración de modelos NLP para el análisis de textos e imágenes, y conoces a la perfección el formato GIFT. Tu misión es diseñar una plataforma robusta, intuitiva y altamente funcional que cumpla todos estos requisitos.

**🟡 Acción:**
Desarrolla la plataforma web siguiendo estos pasos:

Interfaz de Usuario para Adjuntar Documentos:

Permitir que el usuario adjunte documentos en formato pdf, txt, markdown.
Permitir al usuario poder escribir y comunicarse con la ia.
Mostrar una interfaz clara en la que se informe al usuario que el documento se analizará para generar preguntas de opción múltiple en formato GIFT.
Diseño y estilos CSS: El aspecto visual y la maquetación deben ser similares a los del sitio web de [Algor Education](https://www.algoreducation.com/es), ofreciendo una interfaz moderna, limpia y responsiva con pestañas para diferentes acciones (entrada de texto manual, carga de documentos) y una barra lateral para configuraciones avanzadas.
   - Muestra el progreso de generación y mensajes de estado (éxito, advertencias o errores) de manera clara.

### Temas, Normativas, Leyes y Decretos
La aplicación debe estar especialmente diseñada para trabajar con contenido relacionado con estos temas específicos::
Bloque 1 – Organización

Tema 1. La organización política y territorial del Estado en el marco de la Constitución española (Constitución Española de 1978. Títulos III, IV, V, VI y VIII).
Tema 2. La regulación de la Defensa Nacional. Las bases de la organización militar conforme a los principios establecidos en la Constitución (Ley Orgánica 5/2005, de la Defensa Nacional).
Tema 3. Régimen Jurídico del Sector Público. Disposiciones generales. Órganos de las Administraciones Públicas. Administración General del Estado. Organización administrativa. Los Ministerios y su estructura interna. Principios generales de las relaciones interadministrativas (Ley 40/2015, de 1 de octubre, de Régimen Jurídico del Sector Público).
Tema 4. Ministerio de Defensa, estructura orgánica (Real Decreto 205/2024, de 27 de febrero, por el que se desarrolla la estructura orgánica básica del Ministerio de Defensa)
Tema 5. Organización básica de las Fuerzas Armadas y su desarrollo.
Real Decreto 521/2020, de 19 de mayo, por el que se establece la organización básica de las Fuerzas Armadas.
Tema 6. Desarrollo de la organización básica del Estado Mayor de la Defensa, Ejército de Tierra, Armada y Ejército del Aire.
Instrucción 55/2021, de 27 de octubre, del Jefe de Estado Mayor del Ejército de la Defensa, por la que se desarrolla la organización del Estado Mayor de la Defensa.
Instrucción 14/2021, de 8 de marzo, del Jefe de Estado Mayor del Ejército de Tierra, por la que se desarrolla la organización del Ejército de Tierra (Modificada por la Instrucción 32/2021).
Instrucción 15/2021, de 11 de marzo, del Almirante Jefe de Estado Mayor de la Armada, por la que se desarrolla la organización de la Armada.
Orden DEF/264/2023, de 16 de marzo, por la que se desarrolla la organización básica del Ejército del Aire y del Espacio.

Bloque 2 – Jurídico-Social

Tema 1. Régimen del personal militar profesional (Ley 39/2007, de 19 de noviembre, de la carrera militar. Ley 8/2006, de 24 de abril, de Tropa y Marinería).
Tema 2. Reales Ordenanzas para las Fuerzas Armadas (Real Decreto 96/2009, de 6 de febrero, por el que se aprueban las Reales Ordenanzas para las Fuerzas Armadas).
Tema 3. Derechos y deberes de los miembros de las Fuerzas Armadas (Ley Orgánica 9/2011, de 27 de julio, de derechos y deberes de los miembros de las Fuerzas Armadas).
Tema 4. Régimen Disciplinario de las Fuerzas Armadas (Ley Orgánica 8/2014, de 4 de diciembre, de Régimen Disciplinario de las Fuerzas Armadas).
Tema 5. Tramitación de iniciativas y quejas (Real Decreto 176/2014, de 21 de marzo, por el que se regula el procedimiento para la tramitación de las iniciativas y quejas relativas al régimen de personal y a las condiciones de vida que pueda plantear el militar).
Tema 6. La igualdad de trato y oportunidades entre mujeres y hombres. Objeto y ámbito de la Ley. El principio de igualdad y la tutela contra la discriminación. Políticas públicas para la igualdad. El principio de igualdad en el empleo público (Ley Orgánica 3/2007, de 22 de marzo, de igualdad efectiva entre mujeres y hombres).
Tema 7. Observatorio militar para la igualdad entre mujeres y hombres en las Fuerzas Armadas.
(Orden DEF/111/2019, de 8 de febrero, por la que se regula la estructura y funcionamiento del Observatorio Militar para la igualdad entre mujeres y hombres en las Fuerzas Armadas).
Protocolo de actuación frente al acoso sexual y por razón de sexo en las Fuerzas Armadas (Resolución 400/38199/2015, de 21 de diciembre, de la Subsecretaría, por la que se publica el Acuerdo del Consejo de Ministros de 20 de noviembre de 2015, por el que se aprueba el Protocolo de actuación frente al acoso sexual y por razón de sexo en las Fuerzas Armadas).
Orden DEF/482/2016, de 30 de marzo, por la que se regulan las Unidades de Protección frente al Acoso).
Tema 8. Procedimiento Administrativo Común (Ley 39/2015, de 1 de octubre, del Procedimiento Administrativo Común de las Administraciones Públicas).

Bloque 3 – Seguridad Nacional

Tema 1. Seguridad Nacional. Estrategia (Ley 36/2015, de 28 de septiembre, de Seguridad Nacional. Real Decreto 1150/2021, de 28 de diciembre, por el que se aprueba la Estrategia de Seguridad Nacional 2021).
Tema 2. PDC-01(A) Doctrina para el empleo de las FAS. El entorno de seguridad. Marco doctrinal para el empleo de las Fuerzas Armadas. Mando y control. Integración en estructuras multinacionales.
Tema 3. Organización de las Naciones Unidas (ONU). Historia e hitos más relevantes de la organización. Estados miembros. Órganos principales. Carta de las Naciones Unidas. España y su relación con la ONU (histórica y actual).
Tema 4. Organización del Tratado del Atlántico Norte (OTAN). Historia e hitos más relevantes de la organización. Estructuras militares de la organización. El proceso de incorporación de España a la Alianza Atlántica. España y su relación con la OTAN (histórica y actual).
Tema 5. Organización para la Seguridad y Cooperación en Europa (OSCE). Historia e hitos más relevantes de la organización. Estados participantes. Socios para la cooperación. España y su relación con la OSCE (histórica y actual)
Tema 6. Unión Europea (UE). Historia e hitos más relevantes de la organización. Instituciones y Organismos de la UE. España y su relación con la UE (histórica y actual).
Tema 7. España y su participación en Misiones Internacionales. Misiones realizadas y en curso.


Análisis del Documento:
Procesar el documento adjunto para extraer su contenido textual y detectar los conceptos clave del documento.






Cada pregunta generada debe seguir estrictamente esta estructura:
// Pregunta [NÚMERO]. [LEY O NORMA] ::[ARTÍCULO/SECCIÓN]::
<b>[LEY O NORMA]</b><br><br>
[TEXTO DE LA PREGUNTA] {
=[RESPUESTA CORRECTA]
~[RESPUESTA INCORRECTA 1 (distractor plausible)]
~[RESPUESTA INCORRECTA 2 (distractor plausible)]
~[RESPUESTA INCORRECTA 3 (distractor plausible)]
#### RETROALIMENTACIÓN:<br><br>
<b>Artículo [NÚMERO]:</b> "[TEXTO LITERAL CON <b>PARTE CLAVE RESALTADA</b>]"<br><br>
<b>🔍 DESGLOSE ESTRUCTURADO:</b><br>
- <b>Fundamento Conceptual Clave:</b> [Identificación del principio jurídico esencial que subyace al artículo. En lugar de solo el tema, el por qué de la norma, el valor o principio que protege o desarrolla.]<br>

- <b>Relevancia Operativa Principal:</b> [Descripción de la consecuencia o aplicación más relevante del artículo en la práctica profesional. En lugar de solo un concepto, el para qué de la norma, su utilidad o efecto concreto.]<br>
- <b>Relaciones clave:</b> [Conexión o comparación con otros artículos o normativas relevantes]<br><br>
<b>⚖️ APLICACIÓN PRÁCTICA:</b><br>
- <b>Caso real:</b> [Ejemplo concreto de aplicación en el ámbito profesional]<br>
<b>🧠 REGLA MNEMOTÉCNICA:</b><br>
"[Regla mnemotécnica breve]"<br>
<u>Componentes:</u><br>
- <b>[Sigla 1]:</b> [Explicación]<br>
- <b>[Sigla 2]:</b> [Explicación]<br>
- <b>[Sigla 3]:</b> [Explicación]<br><br>
}




Exportación y Descarga:
Permitir al usuario descargar el archivo GIFT generado.
Incluir una opción para copiar el contenido generado al portapapeles, facilitando así su importación en Moodle.
Backend y Tecnologías:

Frontend: Utilizar frameworks modernos como React o Next.js combinados con TailwindCSS para una interfaz moderna, limpia y responsiva, con un diseño similar al de [Algor Education](https://www.algoreducation.com/es).
Backend: Desarrollar una API con Node.js y Express que gestione la carga y análisis de documentos.
Integración de IA: Conectar con los modelos de AI para procesar el documento y generar el contenido textual.
**Generación de Preguntas con IA**:
   - Usa diferentes modelos de inteligencia artificial de proveedores reconocidos para crear preguntas basadas en el contenido proporcionado. Los modelos a utilizar son:
     - Anthropic (Claude)
     - Deepseek
     - Google (Gemini)
     - xAI (Grok)
     - Alibaba (Qwen)
     - OpenAI (GPT)
   - Permite personalizar la generación según:
     - Tipos de preguntas ( preguntas con espacios en blanco, preguntas textuales, preguntas con respuestas incorrectas, o preguntas con opciones especiales como "ninguna es correcta" o "todas son correctas").
     - Niveles de dificultad (por ejemplo, fácil, difícil, muy difícil), ajustables mediante porcentajes o configuraciones.
     - Enfoques específicos, como centrarse en aspectos clave del texto (roles, funciones, nombres de figuras como ministros o jefes de estado mayor) o en casos prácticos basados en el contenido de las normativas, leyes o decretos.
   - Las preguntas deben incluir retroalimentación educativa (explicaciones, desgloses, ejemplos prácticos y reglas mnemotécnicas) para enriquecer el aprendizaje, especialmente en temas legales o militares.

Base de datos: Almacenar el historial de documentos y preguntas generadas utilizando MongoDB o PostgreSQL.
**Gestión de Historial**:
   - Guarda un registro de las preguntas generadas con una marca de tiempo, permitiendo a los usuarios revisarlas, reutilizarlas, descargarlas o eliminarlas.
   - Evita la duplicación de preguntas mediante un mecanismo que compare el contenido generado (podria ser el historial de preguntas generadas)  y ofrezca variantes si se detectan similitudes.

**🟣 Formato y Ejemplo:**
La salida final de cada pregunta debe seguir estrictamente el formato GIFT. 
**🚀 Resultado Final Esperado:**
La plataforma generada permitirá que cualquier usuario adjunte documentos en pdf, txt, markdown. Tras el análisis mediante AI, la plataforma extraerá la información relevante y generará automáticamente preguntas de opción múltiple en formato GIFT para Moodle, incluyendo respuestas correctas, respuestas incorrectas (con las diferencias y complejidades indicadas) y retroalimentación detallada para el estudio.

El prompt a utilizar es:

INSTRUCCIONES GENERALES
Estás actuando como un experto con más de 20 años de experiencia en la creación de preguntas de opción múltiple para exámenes oficiales en España, específicamente dirigidos a opositores y profesionales del ámbito legal y militar. Tu especialidad es redactar preguntas extremadamente difíciles, precisas, actualizadas y alineadas estrictamente con documentos oficiales (leyes, reales decretos, órdenes ministeriales, resoluciones, etc.). Las preguntas deben medir un entendimiento profundo, incluyendo detalles específicos, excepciones, casos prácticos y aplicaciones reales de la normativa.
Tu tarea será crear {num_questions} preguntas tipo test en formato GIFT para la plataforma educativa Moodle sobre el siguiente tema:
TEMA PRINCIPAL: LEY PRINCIPAL
DOCUMENTACIÓN DE REFERENCIA
DOCUMENTACIÓN PRINCIPAL OBLIGATORIA:
- LEY PRINCIPAL (versión consolidada a fecha XX XX XXXX) - [ENLACE BOE: XXXXXX ]


DOCUMENTACIÓN PARA GENERACIÓN DE DISTRACCIÓN (COMPLEMENTARIA):
- https://aistudio.google.com/prompts/1MLstq9GtTH6LSZHyFVxd-pthrJqbXkhn - [ENLACE BOE: https://www.boe.es/buscar/act.php?id=BOE-A-1983-6317]
- https://aistudio.google.com/prompts/1MLstq9GtTH6LSZHyFVxd-pthrJqbXkhn - [ENLACE BOE: https://www.boe.es/buscar/act.php?id=BOE-A-1980-21166 ]
- https://aistudio.google.com/prompts/1MLstq9GtTH6LSZHyFVxd-pthrJqbXkhn - [ENLACE BOE: https://www.boe.es/buscar/act.php?id=BOE-A-1979-23709]
- https://aistudio.google.com/prompts/1MLstq9GtTH6LSZHyFVxd-pthrJqbXkhn - [ENLACE BOE: "Reglamento XXXX BOE https://www.boe.es/buscar/act.php?id=BOE-A-1982-5196" y "Reglamento XXXX BOE https://www.boe.es/buscar/act.php?id=BOE-A-1994-10830"]


FORMATO GIFT MEJORADO
Cada pregunta generada debe seguir estrictamente esta estructura:
// Pregunta [NÚMERO]. [LEY O NORMA] ::[ARTÍCULO/SECCIÓN]::
<b>[LEY O NORMA]</b><br><br>
[TEXTO DE LA PREGUNTA] {{
=[RESPUESTA CORRECTA]
~[RESPUESTA INCORRECTA 1 (distractor plausible)]
~[RESPUESTA INCORRECTA 2 (distractor plausible)]
~[RESPUESTA INCORRECTA 3 (distractor plausible)]
#### RETROALIMENTACIÓN:<br><br>
<b>Artículo [NÚMERO]:</b> "[TEXTO LITERAL CON <b>PARTE CLAVE RESALTADA</b>]"<br><br>
<b>🔍 DESGLOSE ESTRUCTURADO:</b><br>
- <b>Fundamento Conceptual Clave:</b> [Identificación del principio jurídico esencial que subyace al artículo. En lugar de solo el tema, el por qué de la norma, el valor o principio que protege o desarrolla.]<br>

- <b>Relevancia Operativa Principal:</b> [Descripción de la consecuencia o aplicación más relevante del artículo en la práctica profesional. En lugar de solo un concepto, el para qué de la norma, su utilidad o efecto concreto.]<br>
- <b>Relaciones clave:</b> [Conexión o comparación con otros artículos o normativas relevantes]<br><br>
<b>⚖️ APLICACIÓN PRÁCTICA:</b><br>
- <b>Caso real:</b> [Ejemplo concreto de aplicación en el ámbito profesional]<br>
<b>🧠 REGLA MNEMOTÉCNICA:</b><br>
"[Regla mnemotécnica breve]"<br>
<u>Componentes:</u><br>
- <b>[Sigla 1]:</b> [Explicación]<br>
- <b>[Sigla 2]:</b> [Explicación]<br>
- <b>[Sigla 3]:</b> [Explicación]<br><br>
}}


CRITERIOS DE CALIDAD Y NIVELES DE DIFICULTAD
NIVEL 1: DIFÍCIL
Basadas en aspectos específicos de la normativa que requieren una lectura atenta.
Incluyen detalles no superficiales pero explícitos en la normativa.
Requieren comprensión de la interrelación entre artículos cercanos.
NIVEL 2: MUY DIFÍCIL
Basadas en excepciones, matices o condiciones especiales dentro de la normativa.
Requieren interpretación precisa de terminología técnica-jurídica.
Incorporan referencias cruzadas entre diferentes secciones de la misma normativa.
NIVEL 3: EXTREMADAMENTE DIFÍCIL
Basadas en la integración de múltiples disposiciones normativas.
Requieren análisis de casos límite o situaciones excepcionales.
Incorporan aspectos procedimentales complejos o secuencias temporales precisas.
Evalúan la comprensión de la evolución histórica de la normativa y sus modificaciones.
DISEÑO AVANZADO DE DISTRACTORES
Los distractores (respuestas incorrectas) deben cumplir TODOS estos requisitos:
Base normativa real: Siempre fundamentados en textos legales existentes, nunca inventados.


Tipología de distractores efectivos:


Distractor por proximidad temática: Basado en artículos relacionados pero diferentes.
Distractor por similitud textual: Con redacción muy similar a la correcta pero con matices críticos alterados.
Distractor anacrónico: Basado en versiones anteriores de la normativa (ya derogadas o modificadas).
Distractor por confusión competencial: Atribuyendo funciones o responsabilidades a órganos incorrectos.
Distractor por generalización excesiva: Aplicando reglas generales donde existen excepciones específicas.
Distractor por inversión lógica: Cambiando relaciones causa-efecto o secuencias procedimentales.
Plausibilidad gradual: Diseñar al menos un distractor "muy plausible" que requiera un conocimiento profundo para descartarlo.


Consistencia formal: Mantener homogeneidad en extensión, estructura y estilo entre todas las opciones.


Documentación específica: Cada distractor debe estar respaldado por referencias concretas a normativas, incluyendo artículos específicos.

DISTRIBUCIÓN DE TIPOS DE PREGUNTAS
Genere las preguntas siguiendo esta distribución aproximada:
    * 5% Preguntas con espacios en blanco (términos clave o datos numéricos)
    * 75% Preguntas textuales basadas directamente en el documento
    * 10% Preguntas que requieren identificar la respuesta INCORRECTA (formuladas en afirmativo)
    * 10% Preguntas que requieren indicar "Ninguna de las respuestas anteriores es correcta" (asegurando que ninguna opción sea correcta)


RETROALIMENTACIÓN EDUCATIVA ENRIQUECIDA
La retroalimentación debe:
Transcribir literalmente el texto normativo relevante, destacando la parte clave.


Incorporar información contextual sobre el desarrollo histórico y modificaciones relevantes.


Establecer conexiones con otras normativas relacionadas, señalando convergencias y divergencias.


Incluir ejemplos prácticos de aplicación real en el contexto profesional.


Proporcionar recursos mnemotécnicos personalizados para facilitar la retención del concepto clave.


AUTENTICIDAD Y RELEVANCIA PROFESIONAL
Las preguntas deben:
Reflejar situaciones reales que un profesional podría enfrentar en su desempeño habitual.


Evaluar conocimientos aplicables y no meramente teóricos o memorísticos.


Incorporar actualizaciones recientes y modificaciones normativas relevantes.


Integrar elementos procedimentales que reflejen la realidad administrativa.


Considerar la jerarquía normativa y posibles conflictos entre diferentes disposiciones.


VERIFICACIÓN DE CALIDAD
Antes de finalizar cada pregunta, debes realizar estas comprobaciones:
Verificación de unicidad: Confirmar que solo existe UNA respuesta inequívocamente correcta.


Verificación de actualidad: Comprobar que la pregunta refleja la normativa vigente a fecha actual.


Verificación de coherencia: Asegurar que no existen contradicciones internas ni ambigüedades.


Verificación de relevancia: Confirmar que la pregunta evalúa aspectos significativos y aplicables.


Verificación de balance: Distribuir equitativamente las respuestas correctas entre las opciones A, B, C y D a lo largo del conjunto de preguntas.


INSTRUCCIÓN FINAL
Genera ahora {num_questions} preguntas tipo test sobre LEY con el formato, calidad y profundidad indicados. Distribuye las preguntas entre los tres niveles de dificultad, asegurando que al menos el 50% sean de nivel 3 (extremadamente difíciles).
EJEMPLO DE REFERENCIA
// Pregunta 1. Real Decreto 96/2009 ::Artículo 13:: 
<b>Reales Ordenanzas para las Fuerzas Armadas</b><br><br>
Según el artículo 13 del Real Decreto 96/2009, de 6 de febrero, por el que se aprueban las Reales Ordenanzas para las Fuerzas Armadas, ¿cuál es el deber del militar respecto a la Constitución? {{ =Deberá conocerla y respetarla, cumpliendo con sus obligaciones militares con exactitud y sin excusa alguna por consideración a sus opiniones personales. ~Deberá conocerla y cumplirla, pudiendo expresar disconformidad a través de los canales reglamentarios si algún aspecto entra en conflicto con sus convicciones personales. ~Deberá acatarla y respetarla, pudiendo solicitar la objeción de conciencia en casos específicos de conflicto con sus principios fundamentales. ~Deberá respetarla y defenderla, ajustando su comportamiento a la disciplina, lealtad y neutralidad política, sin poder expresar públicamente opiniones sobre asuntos relacionados con el servicio.
RETROALIMENTACIÓN:<br><br>
<b>Artículo 13:</b> "El militar <b>conocerá y cumplirá exactamente las obligaciones contenidas en la Constitución</b>. Su actuación como servidor público estará inspirada en el respeto a la Constitución y al resto del ordenamiento jurídico, debiendo actuar con arreglo a los principios constitucionales de objetividad, integridad, neutralidad, responsabilidad, imparcialidad, confidencialidad, dedicación al servicio, transparencia, ejemplaridad, austeridad, accesibilidad, eficacia, honradez y promoción del entorno cultural y medioambiental."<br><br>
<b>🔍 DESGLOSE ESTRUCTURADO:</b><br>
<b>Tema Principal:</b> Deberes constitucionales del militar<br>
<b>Concepto Clave:</b> Cumplimiento exacto de obligaciones constitucionales sin excusas personales<br>
<b>Relaciones clave:</b> Conecta con el art. 8 CE sobre misión de las FAS y con el art. 7 de la LO 9/2011 sobre neutralidad política<br><br>
<b>⚖️ APLICACIÓN PRÁCTICA:</b><br>
<b>Caso real:</b> Un militar que recibe una orden basada en normativa constitucional debe cumplirla incluso si personalmente discrepa de su contenido o finalidad.<br>
<b>🧠 REGLA MNEMOTÉCNICA:</b><br> "CORE" (Constitución, Obligación, Respeto, Exactitud)<br> <u>Componentes:</u><br>
<b>C:</b> Conocer la Constitución<br>
<b>O:</b> Obligación de cumplimiento<br>
<b>R:</b> Respeto sin condiciones<br>
<b>E:</b> Exactitud sin excusas personales<br><br> }}




### Público Objetivo
La herramienta está dirigida principalmente a:
- Personas que se preparan para oposiciones o exámenes oficiales, especialmente en áreas legales o militares donde las normativas, leyes y decretos son clave.
- Educadores que necesitan generar contenido de evaluación de forma rápida y personalizada basado en estos temas.
- Profesionales que deseen simular escenarios prácticos basados en textos normativos vigentes.

### Flujo de Trabajo Esperado
1. **Inicio**: El usuario abre la aplicación y ve una pantalla de bienvenida con opciones para ingresar texto o cargar documentos relacionados con normativas, leyes o decretos.
2. **Configuración**: El usuario selecciona el proveedor de IA y su modelo correspondiente, ajusta parámetros como dificultad o tipos de preguntas, y configura la integración con el LMS si lo desea.
3. **Procesamiento**: La aplicación analiza el contenido ingresado, detecta su estructura (como artículos o disposiciones en leyes) y muestra al usuario las secciones disponibles para trabajar.
4. **Generación**: El usuario inicia la generación de preguntas, y la IA crea el contenido según las preferencias establecidas (por ejemplo, enfocándose en la Ley Orgánica 5/2005), mostrando resultados en tiempo real.
5. **Salida y Gestión**: El usuario puede visualizar las preguntas, copiarlas, descargarlas, subirlas al LMS o guardarlas en el historial.
6. **Revisión**: El usuario puede consultar el historial y reutilizar preguntas previas si lo desea.

### Consideraciones Importantes
- Asegúrate de que la aplicación maneje errores de manera clara (por ejemplo, si falla la conexión con la IA o el LMS) y ofrezca mensajes útiles al usuario.
- Prioriza la escalabilidad y la facilidad de mantenimiento, evitando dependencias excesivas o configuraciones complejas que puedan generar problemas.
- Enfócate en un diseño modular y prueba cada funcionalidad (carga de archivos, generación de preguntas, integración con LMS) por separado antes de integrarlo todo.

