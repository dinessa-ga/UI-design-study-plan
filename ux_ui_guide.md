# Guía Completa para Proceso de Selección UI/UX Design

## Índice
1. [UX/UI Design](#1-uxui-design)
2. [Attention to Detail (Visual)](#2-attention-to-detail-visual)
3. [Figma](#3-figma)
4. [Design Thinking](#4-design-thinking)
5. [Custom Questions](#5-custom-questions)
6. [Recursos Finales](#recursos-finales)

---

# 1. UX/UI Design

## 1.1 Fundamentos UX/UI

### UX (User Experience) - La Experiencia Completa

La UX es TODO el viaje del usuario con tu producto:
- Emociones que genera
- Facilidad de uso
- Utilidad real
- Accesibilidad
- Rendimiento

#### Componentes de UX

**A) Investigación de Usuarios**

**Métodos cuantitativos:**
- Encuestas (Google Forms, Typeform)
- Analytics (Google Analytics, Hotjar)
- A/B Testing
- Métricas: tasa de conversión, tiempo en tarea, tasa de error

**Métodos cualitativos:**
- Entrevistas 1-a-1 (5-8 usuarios es suficiente)
- Observación contextual
- Card sorting
- Usability testing

**Ejemplo práctico:**
```
App de delivery:
Cuantitativo: "80% abandona el carrito en paso 3"
Cualitativo: "Los usuarios dicen: 'No sé si puedo cambiar la dirección después'"
```

**B) Arquitectura de Información (IA)**

**Principios de Organización:**

1. **Por categoría**: "Electrónica > Celulares > iPhone"
2. **Por tarea**: "Comprar > Vender > Intercambiar"
3. **Por audiencia**: "Para estudiantes > Para empresas"

**Tipos de Navegación:**
- **Global**: Menú principal (siempre visible)
- **Local**: Sub-menús (contextuales)
- **Contextual**: Links relacionados
- **Breadcrumbs**: "Inicio > Productos > Laptops"

**Ejercicio práctico: App de recetas**

```
Opción A (por categoría):
├── Desayunos
├── Almuerzos
├── Cenas
└── Postres

Opción B (por tarea):
├── Buscar recetas
├── Mis favoritas
├── Crear nueva
└── Planear menú semanal

Opción C (híbrida) ✓ MEJOR:
├── Explorar (categorías)
├── Mi cocina (favoritas, historial)
└── Planificar (menú semanal)
```

**C) Flujos de Usuario (User Flows)**

**Componentes:**
- Entry point: ¿Dónde empieza?
- Actions: Qué hace el usuario
- Decision points: Bifurcaciones
- Success state: Meta cumplida
- Error states: Qué pasa si falla

**Template de flujo:**
```
[Usuario nuevo registrándose]

1. Landing page
   ↓
2. Click "Registrarse"
   ↓
3. Formulario registro
   ├─→ ¿Todos los campos válidos?
   │   ├─→ No → Mensaje de error + mantener datos
   │   └─→ Sí → Continuar
   ↓
4. Verificación email
   ├─→ ¿Verificó en 24hrs?
   │   ├─→ No → Reenviar link
   │   └─→ Sí → Continuar
   ↓
5. Onboarding (3 pantallas)
   ↓
6. Dashboard principal ✓
```

### UI (User Interface) - La Capa Visual

**A) Jerarquía Visual**

**Niveles de jerarquía:**
```
Título principal (H1):
- Tamaño: 32-48px
- Weight: Bold (700)
- Color: Más oscuro/contrastado
- Espaciado: Más aire alrededor

Subtítulo (H2):
- Tamaño: 24-32px
- Weight: Semibold (600)
- Color: Mismo tono, ligeramente más claro

Texto cuerpo:
- Tamaño: 16-18px (nunca menos de 16 en móvil)
- Weight: Regular (400)
- Line-height: 1.5-1.7

Texto secundario:
- Tamaño: 14px
- Weight: Regular
- Color: Gris medio (60-70% opacidad)
```

**Ejercicio: Rediseño con jerarquía**

```
ANTES (todo igual):
Receta de Tacos
Tiempo de preparación 30 minutos
Ingredientes tortillas carne cebolla cilantro

DESPUÉS (con jerarquía):
RECETA DE TACOS [H1, 36px, Bold]
⏱ 30 minutos [icono + texto, 14px, gris]

Ingredientes [H2, 24px, Semibold]
• Tortillas de maíz
• 500g carne molida
[16px, Regular, lista]
```

**B) Sistema de Color**

**Paso 1: Paleta base**

```
Primary: Color principal de marca
- P-900: Versión muy oscura
- P-700: Versión oscura
- P-500: Color base (botones principales)
- P-300: Versión clara
- P-100: Muy claro (backgrounds)

Secondary: Color de acento

Neutral: Grises
- N-900: Negro de texto (#1a1a1a)
- N-700: Texto secundario
- N-500: Texto deshabilitado
- N-300: Bordes
- N-100: Backgrounds
- N-50: White (#ffffff)

Semantic: Significado universal
- Success: Verde (#10b981)
- Warning: Amarillo/Naranja (#f59e0b)
- Error: Rojo (#ef4444)
- Info: Azul (#3b82f6)
```

**Paso 2: Reglas de contraste WCAG**

```
Niveles de conformidad:
- AA: 4.5:1 para texto normal (mínimo legal)
- AA: 3:1 para texto grande (18px+ o 14px bold+)
- AAA: 7:1 para texto normal (ideal)

Verificar en: webaim.org/resources/contrastchecker/

Ejemplo:
✗ MAL: Texto gris #999 sobre blanco = 2.8:1
✓ BIEN: Texto gris #666 sobre blanco = 5.7:1
✓ MEJOR: Texto #1a1a1a sobre blanco = 16:1
```

**C) Tipografía**

**Scale tipográfica (Modular Scale):**

```
Ratio 1.25 (Major Third):

Base: 16px
↓ ×1.25
20px (pequeños títulos)
↓ ×1.25
25px (subtítulos H3)
↓ ×1.25
31px (subtítulos H2)
↓ ×1.25
39px (títulos H1)
↓ ×1.25
49px (hero titles)
```

**Combinar fuentes:**

```
Opción 1 - Contraste (común):
- Títulos: Serif (Playfair, Merriweather)
- Cuerpo: Sans-serif (Inter, Roboto)

Opción 2 - Armonía:
- Todo Sans-serif, diferentes weights
- Títulos: Poppins Bold
- Cuerpo: Poppins Regular

Opción 3 - Personalidad:
- Títulos: Display (Bebas Neue)
- Cuerpo: Sans-serif neutro (Inter)

❌ Evita: Dos Sans-serif similares
```

**Recursos:** Google Fonts, fontpair.co

## 1.2 Leyes de UX

### Ley de Fitts
*"El tiempo para alcanzar un objetivo depende de la distancia y tamaño"*

**Aplicación:**
```
✗ MAL: Botón "Pagar" 32×32px en esquina
✓ BIEN: Botón "Pagar" full-width, 48px alto, parte inferior

Regla: Botones primarios mínimo 44×44px
```

### Ley de Hick
*"El tiempo de decisión aumenta con el número de opciones"*

**Aplicación:**
```
✗ MAL: Menú con 15 opciones al mismo nivel
✓ BIEN: 4-5 categorías principales con subcategorías

Regla: Max 7±2 opciones por nivel (Miller's Law)
```

### Ley de Jakob
*"Los usuarios pasan más tiempo en OTROS sitios"*

**No reinventes patrones:**
- Logo en esquina superior izquierda = Home
- Hamburger menu (≡) = Menú
- Lupa (🔍) = Buscar
- Carrito (🛒) = E-commerce
- Corazón (❤️) = Favoritos

**Cuándo romper:** Solo si tu solución es significativamente mejor

### Principios de Gestalt

**1. Proximidad:** Elementos cercanos se perciben relacionados
```
✗ MAL:
[Imagen]
[Texto]    ← 40px separación
[Precio]

✓ BIEN:
[Imagen]
[Texto]    ← 8px
[Precio]   ← 4px
           ← 32px hasta siguiente producto
```

**2. Similitud:** Elementos similares se perciben agrupados
- Todos los botones primarios: mismo color, estilo, tamaño

**3. Ley de Prägnanz:** El cerebro interpreta formas de la manera más simple

## 1.3 Ejercicios Prácticos

### Ejercicio 1: Jerarquía Visual

**Mejora este diseño de tarjeta:**

```
ANTES:
────────────────────
│ iPhone 15 Pro    │
│ $999             │
│ Disponible       │
│ [Comprar]        │
────────────────────

DESPUÉS:
────────────────────
│ iPhone 15 Pro     │ ← 24px, Bold
│                   │
│ $999              │ ← 32px, Bold, primary color
│ Disponible • Stock: 5 │ ← 12px, gris
│                   │
│ [COMPRAR AHORA]   │ ← Full-width button
────────────────────
```

### Ejercicio 2: Rediseño con Principios UX

**Analiza este flujo problemático:**

```
App de reserva de restaurantes:

PROBLEMAS:
1. 50 restaurantes listados (Ley de Hick)
2. 30 platos en cada uno (sobrecarga)
3. Formulario con 12 campos (fricción)
4. Botón "Confirmar" en esquina (Ley de Fitts)

SOLUCIÓN:
1. Home: Búsqueda + 6 destacados + filtros
2. Menú categorizado (4 categorías)
3. Formulario: 4 campos esenciales
4. Botón sticky en bottom, full-width
```

---

# 2. Attention to Detail (Visual)

## 2.1 Metodología de Escaneo Visual

**Técnica "Grid Mental":**

```
Divide la pantalla en cuadrícula 3×3:

[1] [2] [3]
[4] [5] [6]
[7] [8] [9]

Escanea sistemáticamente: 1→2→3, luego 4→5→6, luego 7→8→9
```

## 2.2 Checklist de Revisión

**Alineación:**
- [ ] Todos los textos alineados a misma guía
- [ ] Iconos centrados verticalmente con texto
- [ ] Elementos de lista con mismo indent
- [ ] Márgenes consistentes en todos los lados

**Espaciado:**
- [ ] Sistema 8pt aplicado (0, 8, 16, 24, 32, 40, 48...)
- [ ] Padding interno consistente
- [ ] Margin entre secciones idéntico
- [ ] Line-height uniforme

**Tipografía:**
- [ ] Mismo font-family en elementos similares
- [ ] Font-sizes consistentes
- [ ] Font-weights correctos
- [ ] Letter-spacing correcto

**Color:**
- [ ] Valores HEX exactos (no mezclar #3366ff y #3465ff)
- [ ] Opacity consistente
- [ ] Estados hover/active definidos
- [ ] Contraste WCAG cumplido

**Iconografía:**
- [ ] Mismo estilo (todos outline o todos filled)
- [ ] Mismo tamaño base
- [ ] Mismo stroke-width
- [ ] Alineados con texto

## 2.3 Ejercicios de Entrenamiento

### Ejercicio 1: Encuentra las diferencias

```
VERSIÓN A vs VERSIÓN B - Busca 5 diferencias:

Diferencias típicas:
1. Espaciado entre logo e iconos
2. Tamaño de títulos
3. Color de precios
4. Márgenes
5. Weights de texto
```

### Ejercicio 2: Spot the Bug

```
Analiza este botón:
[  Continuar  ] ← 12px padding left
                  16px padding right

PROBLEMA: Padding asimétrico
SOLUCIÓN: 16px en ambos lados
```

### Ejercicio 3: Práctica Real

1. Ve a Dribbble.com
2. Elige un diseño
3. Memorízalo 30 segundos
4. Cierra los ojos
5. Describe:
   - Colores principales
   - Cantidad de elementos
   - Ubicación del CTA
   - Tipografías

### Ejercicio 4: Pixel Perfect Challenge

En Figma, crea:
```
Dos rectángulos:
- 200px × 100px
- Espaciados 24px exacto
- Color #3B82F6
- Border radius 8px
- Sombra: 0px 4px 12px rgba(0,0,0,0.1)

Duplica y verifica que sean IDÉNTICOS
```

## 2.4 Herramientas

**En Figma:**
- Rulers (Shift + R): Ver alineación
- Pixel Grid (Cmd/Ctrl + '): Ver pixels exactos
- Measure plugin: Distancias precisas
- Stark plugin: Contraste automático

**Apps de Entrenamiento:**
- Can't Unsee (cantunsee.space): Game de diseño
- Betterwebtype.com: Ejercicios de tipografía

---

# 3. Figma

## 3.1 Fundamentos Esenciales

### Frames vs Groups

**GROUPS (Cmd/Ctrl + G):**
- Simplemente agrupa elementos
- No tiene propiedades de layout
- El tamaño es la suma de sus hijos
- Útil para: Organizar capas rápidamente

**FRAMES (F):**
- Es un contenedor con propiedades
- Puede tener Auto Layout
- Puede tener Constraints
- Puede exportarse independientemente
- Puede tener Clips content

**Regla de oro:**
- Usa FRAMES para: Componentes, Pantallas, Secciones
- Usa GROUPS para: Organización temporal

### Auto Layout - El Superpoder

**Qué es:** Sistema de layout responsivo (como CSS Flexbox)

**Cómo activarlo:**
- Método 1: Selecciona elementos → Shift + A
- Método 2: Frame con elementos → Click "+" en Auto Layout

**Propiedades principales:**

```
1. Direction (Dirección):
   Horizontal →: [Button] [Button] [Button]
   Vertical ↓:   [Button]
                 [Button]
                 [Button]

2. Spacing (Espaciado):
   0px  → [Item][Item][Item]
   16px → [Item]    [Item]    [Item]
   Auto → [Item]              [Item]

3. Padding:
   16px all sides = espacio interno

4. Alignment:
   Packed: Elementos juntos
   Space between: Máxima separación
```

### EJERCICIO: Botón responsivo

```
Paso 1: Crea Frame (F)
Paso 2: Agrega texto "Comprar ahora"
Paso 3: Shift + A (Auto Layout)
Paso 4: Configura:
   - Padding: 16px horizontal, 12px vertical
   - Alignment: Center/Center

Paso 5: Duplica texto → "Comprar ahora mismo"
El botón se expande automáticamente! 🎉
```

### EJERCICIO AVANZADO: Card con Auto Layout

```
1. Frame principal (Auto Layout vertical, spacing: 16px)
   ├── Image (Fixed height: 200px)
   ├── Frame "Content" (Auto Layout vertical, spacing: 8px)
   │   ├── Text "Título"
   │   ├── Text "Descripción"
   │   └── Frame "Meta" (Auto Layout horizontal, spacing: 8px)
   │       ├── Text "4.5 ★"
   │       └── Text "1.2k reviews"
   └── Button (Auto Layout, full width)

Propiedades:
- Padding: 16px
- Width: Fixed 320px
- Height: Hug contents
```

## 3.2 Components & Variants

### Crear un Component System

**Paso 1: Component básico**

```
Crea un botón:
1. Frame con Auto Layout
2. Texto "Label"
3. Padding 16×12
4. Background #3B82F6
5. Border radius 8px
6. Cmd/Ctrl + Alt + K (Create component)
```

**Paso 2: Variants**

```
Create variants con propiedades:

Properties:
- State: Default, Hover, Disabled
- Size: Small, Medium, Large
- Icon: None, Leading, Trailing

Variantes automáticas:
3 states × 3 sizes × 3 icon options = 27 variantes
```

### Component Properties

**Boolean Properties:**
```
Ejemplo: Mostrar/ocultar icono

Property: "Show icon"
Tipo: Boolean
Default: True

En instancias:
☑ Show icon = visible
☐ Show icon = oculto
```

**Text Properties:**
```
Property: "Label"
Tipo: Text
Default: "Button text"

En instancias: texto editable
```

**Instance Swap:**
```
Property: "Icon"
Tipo: Instance swap

En instancias: cambia a cualquier icono
```

## 3.3 Constraints - Diseño Responsivo

**Tipos:**
- Left: Fijo a izquierda
- Right: Fijo a derecha
- Left & Right: Se estira horizontalmente
- Center: Centrado
- Scale: Escala proporcionalmente

### EJERCICIO: Navbar responsive

```
Frame "Navbar" (1440px × 64px)

Logo (constraint: Left + Top):
- Fijo a la izquierda

Nav Links (constraint: Center + Top):
- Centrados

Profile (constraint: Right + Top):
- Fijo a la derecha

Prueba redimensionar: 1440→1200→768
```

## 3.4 Styles - Sistema de Diseño

**Color Styles:**
```
1. Dibuja rectángulo
2. Color: #3B82F6
3. Fill → Styles → ➕
4. Nombre: "Colors/Primary/500"

Tu librería:
Colors/Primary/300
Colors/Primary/500
Colors/Primary/700
Colors/Neutral/100
Colors/Neutral/900
```

**Text Styles:**
```
1. Text layer
2. Font: Inter, 32px, Bold
3. Line-height: 40px
4. Styles → ➕
5. Nombre: "Heading/H1"

Tu librería:
Display/Large (56px)
Heading/H1 (32px)
Heading/H2 (24px)
Body/Regular (16px)
Caption (12px)
```

**Effect Styles (Sombras):**
```
1. Frame o Shape
2. Effects → Drop shadow
3. X:0, Y:4, Blur:12, Color: rgba(0,0,0,0.1)
4. Styles → ➕ "Shadow/Small"

Tu librería:
Shadow/Small: 0px 2px 4px
Shadow/Medium: 0px 4px 12px
Shadow/Large: 0px 8px 24px
```

## 3.5 Plugins Esenciales

**Top 10:**
1. **Iconify** - Miles de iconos gratis
2. **Unsplash** - Imágenes placeholder
3. **Stark** - Verificar contraste
4. **Content Reel** - Datos falsos
5. **Autoflow** - Generar flowcharts
6. **Wireframe** - Convertir a wireframes
7. **Remove BG** - Quitar fondos
8. **Chart** - Crear gráficos
9. **Token Studio** - Design tokens
10. **Figma to Code** - Exportar a HTML/React

## 3.6 Atajos de Teclado

**Esenciales:**
```
HERRAMIENTAS:
V - Move
F - Frame
R - Rectangle
O - Ellipse
T - Text
K - Scale
H - Hand

ACCIONES:
Cmd/Ctrl + D - Duplicate
Alt + Drag - Duplicate while dragging
Cmd/Ctrl + G - Group
Cmd/Ctrl + ] - Bring forward
Cmd/Ctrl + [ - Send backward
Cmd/Ctrl + Alt + K - Create component

LAYOUT:
Shift + A - Add Auto Layout
Cmd/Ctrl + ' - Toggle pixel grid
Shift + R - Toggle rulers
```

## 3.7 Ejercicios Prácticos

### Ejercicio 1: Login Screen (15 min)

**Requisitos:**
- Frame 375×812 (iPhone)
- Logo arriba
- 2 inputs (Email, Password)
- Botón "Login"
- Link "¿Olvidaste contraseña?"
- Botones sociales

**Aplica:**
✓ Auto Layout en todo
✓ Components para inputs
✓ Constraints correctos
✓ Color styles
✓ Text styles

### Ejercicio 2: Component System (20 min)

**Crea:**
1. Button (3 variants: Primary, Secondary, Ghost)
2. Input (3 states: Default, Focused, Error)
3. Card (image, title, description, button)

**Usa:**
✓ Variants
✓ Component properties
✓ Auto Layout
✓ Shared styles

### Ejercicio 3: Responsive Dashboard

**Crea frame 1440px:**
- Sidebar (240px fixed)
- Main content (flexible)
  - Header con search
  - Grid de cards (4 columnas)
  - Footer

**Aplica constraints para:**
- 1440px
- 1280px
- 1024px

---

# 4. Design Thinking

## 4.1 Las 5 Fases

### FASE 1: EMPATIZAR (Empathize)

**Objetivo:** Entender profundamente a los usuarios

#### Métodos

**A) Entrevistas en profundidad**

```
Script ejemplo (app fitness):

Introducción (2 min):
"Quiero entender cómo haces ejercicio actualmente."

Preguntas de contexto (5 min):
- ¿Con qué frecuencia haces ejercicio?
- ¿Dónde sueles ejercitarte?

Preguntas de comportamiento (10 min):
- Cuéntame sobre la última vez
- ¿Qué aplicaciones usas?
- ¿Qué te motiva?
- ¿Qué te desmotiva?

Preguntas de dolor (5 min):
- ¿Qué es lo más frustrante?
- ¿Has abandonado alguna rutina? ¿Por qué?

Cierre (3 min):
- ¿Algo más que compartir?
```

**Técnica: "5 Whys"**
```
Usuario: "No uso apps de fitness"
¿Por qué? "Son complicadas"
¿Por qué? "Tienen muchas opciones"
¿Por qué? "No sé cuál elegir"
¿Por qué? "No hay guía para principiantes"
→ INSIGHT: Necesitan onboarding personalizado
```

**B) Observación contextual**

```
Qué observar:
✓ Entorno
✓ Secuencia de acciones
✓ Interrupciones
✓ Frustración
✓ Workarounds
```

**C) User Persona**

```
TEMPLATE:

[Foto]

NOMBRE: María Rodríguez
EDAD: 32 años
OCUPACIÓN: Diseñadora freelance
UBICACIÓN: Ciudad

OBJETIVOS:
1. Mantenerse en forma sin gym
2. Hacer ejercicio en casa (30-45 min)
3. Ver progreso medible

FRUSTRACIONES:
1. Apps muy técnicas
2. Rutinas genéricas
3. Falta de motivación

COMPORTAMIENTO:
"Intento 3 veces/semana pero solo logro 1-2"

TECH SAVVINESS: ████░░ (4/6)
```

### FASE 2: DEFINIR (Define)

**Objetivo:** Sintetizar en un problema claro

**A) Problem Statement**

**Template:**
```
[Usuario] necesita [necesidad] porque [insight]

✗ MAL:
"Los usuarios necesitan mejor app"

✓ BIEN:
"María necesita rutinas guiadas y cortas porque 
trabaja desde casa y se siente abrumada"

✓ MEJOR:
"Profesionales 28-35 años necesitan rutinas sin 
equipo porque carecen de tiempo y conocimiento"
```

**B) Point of View (POV)**

```
[Usuario] necesita [necesidad]
Sorprendentemente, [insight inesperado]

Ejemplo:
"María necesita hacer ejercicio regularmente.
Sorprendentemente, el problema no es tiempo sino 
la cantidad abrumadora de opciones."
```

**C) How Might We (HMW)**

```
Problema → HMW

"Usuarios abandonan por complejidad"
↓
HMW simplificar onboarding?
HMW hacer primer uso memorable?
HMW reducir fricción en primeros 5 min?

"No saben qué ejercicio hacer"
↓
HMW recomendar ejercicio perfecto?
HMW personalizar sin 100 preguntas?
HMW usar IA para adaptar en tiempo real?
```

### FASE 3: IDEAR (Ideate)

**Objetivo:** Generar muchas soluciones

**A) Brainstorming Rules**

```
REGLAS:
1. Cantidad > calidad (50+ ideas en 30 min)
2. No juzgar
3. Construir sobre ideas ("Sí, y además...")
4. Ser visual
5. Ideas locas bienvenidas

❌ PROHIBIDO:
- "Eso no va a funcionar"
- "Ya lo intentamos"
- "Es muy caro/complejo"
```

**B) Crazy 8's**

```
SETUP:
- 1 hoja dividida en 8
- 1 minuto por cuadro
- 8 minutos total

┌─────┬─────┬─────┬─────┐
│  1  │  2  │  3  │  4  │
├─────┼─────┼─────┼─────┤
│  5  │  6  │  7  │  8  │
└─────┴─────┴─────┴─────┘

Minuto 1: Idea obvia
Minuto 2: Variación
Minuto 3: Completamente diferente
Minuto 4: Combinar 1+3
Minuto 5: Idea loca
Minuto 6: Simplificar la loca
Minuto 7: Inspirada por competidor
Minuto 8: Tu favorita mejorada
```

**C) SCAMPER**

```
S - Substitute: ¿Qué reemplazar?
C - Combine: ¿Qué combinar?
A - Adapt: ¿Qué adaptar?
M - Modify: ¿Qué cambiar?
P - Put to another use: ¿Otro uso?
E - Eliminate: ¿Qué quitar?
R - Reverse: ¿Qué invertir?
```

**D) Matriz de Votación**

```
IMPACTO vs ESFUERZO

Alto Impacto │  🔶  │  ⭐  │
             │  💎  │  ⭐  │
─────────────┼──────┼──────┤
Bajo Impacto │  ⚪  │  🔷  │
             │  ⚪  │  🔷  │
             └──────┴──────┘
               Alto   Bajo
                ESFUERZO

⭐ Quick Wins: Hacer primero
🔶 Big Bets: Hacer después
🔷 Maybes: Considerar
⚪ Time Sinks: Evitar
```
