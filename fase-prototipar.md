# FASE 4: PROTOTIPAR (Prototype)

## Objetivo
Hacer las ideas tangibles para poder testarlas con usuarios reales.

---

## Tabla de Contenidos
1. [Niveles de Fidelidad](#niveles-de-fidelidad)
2. [Prototipo en Figma - Paso a Paso](#prototipo-en-figma)
3. [Interacciones Avanzadas](#interacciones-avanzadas)
4. [Micro-interactions](#micro-interactions)
5. [Smart Animate](#smart-animate)
6. [Prototipos para Testing](#prototipos-para-testing)
7. [Ejercicios Prácticos](#ejercicios-prácticos)

---

## Niveles de Fidelidad

### 1. PAPER PROTOTYPE (Fidelidad Ultra-Baja)

**⏱ Tiempo:** 30 minutos  
**📦 Material:** Papel, marcador  
**🎯 Cuándo usar:** Validar flujo básico y arquitectura de información

#### Ventajas
✅ Rapidísimo de crear  
✅ Súper barato (costo casi $0)  
✅ Fácil de iterar (tirar y redibujar)  
✅ Elimina distracciones visuales  
✅ Enfoca conversación en funcionalidad

#### Desventajas
❌ No se puede testear interacción real  
❌ Usuario debe usar imaginación  
❌ Difícil compartir remotamente  
❌ No valida diseño visual

#### Ejemplo Visual
```
┌─────────────────┐
│  [ Logo ]       │
│                 │
│  Bienvenido!    │
│                 │
│  [Botón Start]  │
└─────────────────┘
```

#### Cuándo usar Paper Prototype
- Etapa muy inicial (primeras horas del proyecto)
- Workshop de ideación con stakeholders
- Validar concepto antes de invertir tiempo en diseño
- Necesitas feedback rápido del equipo

---

### 2. WIREFRAME (Fidelidad Baja)

**⏱ Tiempo:** 2-4 horas  
**🛠 Herramienta:** Figma, Balsamiq, Sketch  
**🎯 Cuándo usar:** Validar layout y arquitectura de información

#### Ventajas
✅ Clarifica estructura y jerarquía  
✅ Fácil y rápido de cambiar  
✅ Se enfoca en funcionalidad, no estética  
✅ Compartible digitalmente  
✅ Permite testing remoto básico

#### Desventajas
❌ Usuario no ve branding  
❌ No valida decisiones de color/tipografía  
❌ Puede ser difícil de entender para stakeholders no-técnicos  
❌ No captura la emoción del diseño final

#### Características de un buen wireframe
```
- Usa solo grises/blancos/negros
- Boxes para imágenes
- "Lorem ipsum" o texto placeholder
- Iconos simples (outline)
- Sin sombras ni gradientes
- Sin fotos reales

Elementos típicos:
┌─────────────────────────┐
│ [   Logo   ]  ☰  🔍  👤│ ← Header
├─────────────────────────┤
│                         │
│  Heading Text Here      │ ← Hero
│  Subheading text here   │
│                         │
│  [Call to Action]       │
│                         │
├─────────────────────────┤
│ [IMG] Title             │ ← Content Cards
│       Description       │
│       [Button]          │
├─────────────────────────┤
│ [IMG] Title             │
│       Description       │
│       [Button]          │
└─────────────────────────┘
```

#### Cuándo usar Wireframes
- Después de definir user flows
- Antes de invertir en diseño visual
- Para alinear equipo sobre estructura
- Presentar a stakeholders técnicos
- Documentar arquitectura de información

---

### 3. MOCKUP (Fidelidad Media-Alta)

**⏱ Tiempo:** 1-2 días  
**🛠 Herramienta:** Figma  
**🎯 Cuándo usar:** Validar diseño visual y branding

#### Ventajas
✅ Realista visualmente  
✅ Valida decisiones estéticas  
✅ Útil para presentar a stakeholders  
✅ Genera emoción y buy-in  
✅ Sirve para handoff a desarrollo

#### Desventajas
❌ Toma más tiempo crear  
❌ Usuarios se enfocan en colores, no en flujo  
❌ Cambios son más costosos  
❌ Puede crear falsas expectativas  
❌ Sin interacciones reales

#### Qué incluye un mockup
```
✓ Colores de marca reales
✓ Tipografía final
✓ Imágenes reales o muy realistas
✓ Iconografía consistente
✓ Espaciados exactos (8pt grid)
✓ Sombras y efectos visuales
✓ Estados (default, hover, active, disabled)
✓ Contenido realista (no "lorem ipsum")
```

#### Cuándo usar Mockups
- Después de aprobar wireframes
- Para presentaciones a clientes/ejecutivos
- Cuando necesitas aprobación de branding
- Para documentar design system
- Antes de crear prototipo interactivo

---

### 4. PROTOTIPO INTERACTIVO (Fidelidad Alta)

**⏱ Tiempo:** 3-5 días  
**🛠 Herramienta:** Figma, Framer, ProtoPie  
**🎯 Cuándo usar:** Validar interacciones y micro-animaciones

#### Ventajas
✅ Experiencia casi real  
✅ Valida animaciones y transiciones  
✅ Detecta problemas de UX antes de código  
✅ Perfecto para usability testing  
✅ Impresiona stakeholders  
✅ Reduce malentendidos con developers

#### Desventajas
❌ Requiere más esfuerzo y tiempo  
❌ Puede crear falsas expectativas ("¿ya está listo?")  
❌ Difícil mantener sincronizado con cambios  
❌ No todos los detalles son posibles sin código

#### Qué incluye un prototipo interactivo
```
✓ Todos los elementos de mockup +
✓ Navegación funcional entre pantallas
✓ Animaciones y transiciones
✓ Scroll real
✓ Hover states
✓ Micro-interactions
✓ Feedback visual de acciones
✓ Estados de carga
✓ Mensajes de error
✓ Flujos completos end-to-end
```

#### Cuándo usar Prototipos Interactivos
- Antes de empezar desarrollo
- Para usability testing comprehensivo
- Validar animaciones complejas
- Pitch a inversionistas
- Demos de producto
- Training de equipo de ventas

---

## Comparación Rápida

| Aspecto | Paper | Wireframe | Mockup | Prototipo |
|---------|-------|-----------|--------|-----------|
| **Tiempo** | 30min | 2-4h | 1-2d | 3-5d |
| **Fidelidad Visual** | 0% | 20% | 90% | 95% |
| **Interactividad** | 0% | 0% | 0% | 90% |
| **Costo cambios** | $0 | $ | $$ | $$$ |
| **Mejor para** | Concepto | Estructura | Visual | UX Testing |

---

## Prototipo en Figma

### Proyecto Completo: App de To-Do List

**🎯 Objetivo:** Crear prototipo interactivo funcional en 30-40 minutos

**📱 Screens a diseñar:**
1. Home (lista de tareas)
2. Add Task (crear nueva tarea)
3. Task Detail (ver detalles)

---

### PASO 1: Setup Inicial (5 min)

#### 1.1 Crear Frames
```
1. Presiona F (Frame tool)
2. En panel derecho, selecciona: iPhone 14 Pro (393 × 852)
3. Crea 3 frames:
   - Nombra: "01 - Home"
   - Nombra: "02 - Add Task"
   - Nombra: "03 - Task Detail"

Tip: Mantén 100px de espacio entre frames
```

#### 1.2 Establecer Design System Rápido
```
Colors:
- Primary: #3B82F6 (azul)
- Success: #10B981 (verde)
- Background: #F9FAFB (gris claro)
- Text: #1F2937 (negro)
- Secondary Text: #6B7280 (gris)

Typography:
- H1: Inter Bold 28px
- H2: Inter Semibold 20px
- Body: Inter Regular 16px
- Caption: Inter Regular 14px
```

---

### PASO 2: Diseñar Pantalla Home (15 min)

#### 2.1 Estructura Base
```
Frame "01 - Home":

├── Status Bar (arriba)
│   ├── Hora "9:41"
│   └── Indicadores (señal, wifi, batería)
│
├── Header
│   ├── Título "My Tasks" (H1, left aligned)
│   └── Icon Settings (⚙️, top-right)
│
├── Stats Bar
│   ├── "5 Pending" (caption)
│   └── "3 Completed" (caption, green)
│
├── Add Task Button
│   ├── "+" Icon
│   └── "Add New Task" text
│   └── Auto Layout horizontal, full width
│
└── Task List (Auto Layout vertical, spacing: 12px)
    ├── Task Card 1
    ├── Task Card 2
    └── Task Card 3
```

#### 2.2 Crear Task Card Component

**Task Card estructura:**
```
Frame "Task Card" (Auto Layout):
├── Checkbox (24×24)
├── Content (Auto Layout vertical)
│   ├── Title "Buy groceries" (Body, bold)
│   └── Time "2:00 PM" (Caption, gray)
└── Priority Badge (High/Medium/Low)

Properties:
- Padding: 16px all sides
- Background: White
- Border radius: 12px
- Shadow: 0px 2px 8px rgba(0,0,0,0.08)
- Spacing: 12px
```

**Código visual del Task Card:**
```
┌────────────────────────────────────┐
│ ☐  Buy groceries          [HIGH]  │
│    2:00 PM                         │
└────────────────────────────────────┘
```

#### 2.3 Crear Button "Add Task"

```
1. Frame con Auto Layout
2. Add Icon: "+" (20px, white)
3. Add Text: "Add New Task" (white)
4. Spacing: 8px
5. Padding: 16px horizontal, 14px vertical
6. Background: #3B82F6
7. Border radius: 12px
8. Alignment: Center/Center
9. Width: Fill container
```

---

### PASO 3: Diseñar Pantalla "Add Task" (10 min)

```
Frame "02 - Add Task":

├── Header
│   ├── Back Button "←" (top-left)
│   └── Title "New Task" (center)
│
├── Form (Auto Layout vertical, spacing: 20px)
│   │
│   ├── Input: Task Name
│   │   ├── Label "Task Name"
│   │   └── Text Input Field
│   │
│   ├── Input: Description
│   │   ├── Label "Description (optional)"
│   │   └── Text Area
│   │
│   ├── DateTime Picker
│   │   ├── Label "Date & Time"
│   │   └── Picker Component
│   │
│   └── Priority Selector
│       ├── Label "Priority"
│       └── Pills: [High] [Medium] [Low]
│
└── Bottom Actions
    ├── Button "Cancel" (secondary)
    └── Button "Create Task" (primary)
```

#### Input Field Component
```
Frame "Input Field" (Auto Layout vertical):
├── Label (Caption, gray)
└── Input
    ├── Padding: 12px
    ├── Border: 1px solid #E5E7EB
    ├── Border radius: 8px
    ├── Placeholder text: gray
    ├── States: Default, Focused, Error
```

---

### PASO 4: Diseñar Pantalla "Task Detail" (10 min)

```
Frame "03 - Task Detail":

├── Header
│   ├── Back Button "←"
│   ├── Title "Task Details"
│   └── Edit Button "✏️"
│
├── Content (Auto Layout vertical, spacing: 24px)
│   │
│   ├── Checkbox + Title
│   │   ├── Large Checkbox (32×32)
│   │   └── Title "Buy groceries" (H2)
│   │
│   ├── Details Section
│   │   ├── Row: 📅 "Today, 2:00 PM"
│   │   ├── Row: 🔔 "Remind 30 min before"
│   │   └── Row: ⚠️ Priority: High
│   │
│   ├── Description
│   │   ├── Label "Description"
│   │   └── Text "Get milk, eggs, bread..."
│   │
│   └── Notes Section
│       └── Text area for notes
│
└── Bottom Actions
    ├── Button "Delete" (red, ghost)
    └── Button "Mark Complete" (primary)
```

---

### PASO 5: Conectar Interacciones (10 min)

#### 5.1 Navegación Básica

**Home → Add Task:**
```
1. Selecciona Button "Add New Task" en Home
2. Panel derecho → Tab "Prototype"
3. Click en punto azul del botón
4. Arrastra flecha hasta frame "02 - Add Task"
5. Configura:
   - Interaction: On Click
   - Action: Navigate to
   - Animation: Move In
   - Direction: From Right
   - Easing: Ease Out
   - Duration: 300ms
```

**Add Task → Home (Back):**
```
1. Selecciona Back Button "←"
2. Prototype → Arrastra a "01 - Home"
3. Configura:
   - On Click
   - Navigate to
   - Move Out
   - To Right
   - Ease Out
   - 300ms
```

**Home → Task Detail:**
```
1. Selecciona Task Card
2. Prototype → Arrastra a "03 - Task Detail"
3. Configura:
   - On Click
   - Navigate to
   - Move In
   - From Right
   - Ease Out
   - 300ms
```

#### 5.2 Interacción: Create Task

**Button "Create Task":**
```
1. Selecciona button en "02 - Add Task"
2. Arrastra a "01 - Home"
3. Configura:
   - On Click
   - Navigate to
   - Instant (no animation)
   - After delay: 0ms

Esto simula: crear tarea y volver a home
```

#### 5.3 Interacción: Complete Task

**Checkbox en Task Detail:**
```
1. Selecciona checkbox grande
2. Crea variant del frame con checkbox checked
3. Prototype → Change to variant
4. Animate: Smart Animate
5. Duration: 200ms

Efecto: Checkbox se marca con animación suave
```

---

### PASO 6: Micro-interactions Avanzadas (Bonus)

#### 6.1 Button Hover Effect

**Para botones importantes:**
```
1. Crea component del botón
2. Add variant: State = Hover
3. En Hover variant:
   - Aumenta brightness 10%
   - Scale: 1.02
   - Shadow: Aumenta blur de 8 → 12
4. Prototype:
   - While Hovering → Change to Hover
   - Smart Animate
   - Duration: 200ms
```

#### 6.2 Input Focus State

**Para campos de texto:**
```
1. Component Input con variants
2. Variant: State = Default
3. Variant: State = Focused
4. En Focused:
   - Border color: #3B82F6
   - Border width: 2px
   - Add shadow: 0 0 0 4px rgba(59,130,246,0.1)
5. Prototype:
   - While Pressing → Focused
   - Smart Animate
   - 150ms
```

---

### PASO 7: Preview y Testing (5 min)

#### 7.1 Ejecutar Prototipo
```
1. Click en Play ▶️ (esquina superior derecha)
   O presiona: Cmd/Ctrl + Enter
2. Se abre en nueva ventana
3. Prueba todos los flujos:
   ✓ Home → Add Task → Back
   ✓ Home → Task Detail
   ✓ Create Task
   ✓ Hover effects
```

#### 7.2 Compartir Prototipo
```
1. Click "Share" (arriba derecha)
2. "Copy link"
3. Configurar:
   ✓ Anyone with the link can view
   ✓ Allow comments
   ✓ Show prototype
4. Enviar link a stakeholders/testers
```

---

## Interacciones Avanzadas

### 1. Overlay Modal

**Uso:** Mostrar modal/popup sin cambiar de pantalla

```
Ejemplo: Confirmation Dialog

Setup:
1. Crea frame "Delete Confirmation"
2. Hazlo pequeño (300×200)
3. En pantalla origen, selecciona trigger (e.g. Delete button)
4. Prototype → Arrastra a modal frame
5. Configura:
   - On Click
   - Open Overlay
   - Position: Center
   - Close when clicking outside: ✓
   - Background: Manual
   - Background color: Black 60% opacity
   - Animation: Dissolve
   - Duration: 200ms
```

**Cerrar Overlay:**
```
En modal:
1. Selecciona botón "Cancel" o "X"
2. Prototype → Close Overlay
3. Animation: Dissolve
```

---

### 2. Scroll Behavior

**Para contenido largo:**

```
Setup:
1. Frame contenedor (Fixed height, e.g. 600px)
2. Frame interior con contenido (Height: Hug contents)
3. Selecciona frame contenedor
4. Panel derecho → Prototype
5. Overflow behavior: Vertical scrolling
6. Enable: Horizontal scrolling (si necesario)
```

**Scroll con Snap:**
```
Para carousel/slider:
1. Frame horizontal con cards
2. Overflow: Horizontal scrolling
3. Enable: Snap to position
```

---

### 3. Drag Interaction

**Uso:** Swipe cards, sliders, etc.

```
Ejemplo: Swipe to Delete

Setup:
1. Task Card component con 2 variants:
   - Default (X position: 0)
   - Swiped (X position: -80)
2. Prototype:
   - While dragging → Swiped
   - Horizontal constraint
   - Spring animation
```

---

### 4. Multi-State Components

**Uso:** Buttons con múltiples estados

```
Component: Button
Variants:
├── State: Default
├── State: Hover
├── State: Pressed
├── State: Loading
└── State: Success

Prototype connections:
- While Hovering → Hover
- While Pressing → Pressed
- On Click → Loading
- After 2000ms → Success
```

---

## Micro-interactions

### 1. Button Press Effect

```
Component Button:
- Default: scale 1.0
- Pressed: scale 0.98

Prototype:
- While Pressing → Pressed variant
- Smart Animate
- Duration: 100ms
- Easing: Ease in
```

---

### 2. Success Checkmark Animation

```
Component Checkmark:
- Before: opacity 0, scale 0
- After: opacity 1, scale 1

Prototype:
- On Click → After variant
- Smart Animate
- Duration: 400ms
- Easing: Spring (si disponible) o Ease out bounce
```

---

### 3. Loading Spinner

```
Component Spinner:
- Frame con icon/shape
- Rotation: 0° → 360°

Prototype:
- After delay: 0ms
- Navigate to same frame
- Smart Animate
- Duration: 1000ms
- Loop: ✓ (enable loop)
```

---

### 4. Input Validation

```
Component Input:
Variants:
- Default
- Error
- Success

Prototype:
- On input error → Error variant (border red, shake)
- On valid input → Success variant (border green, checkmark)

Animation for Error:
1. Move slightly left (-4px)
2. Move right (+4px)
3. Move center (0)
Duration: 400ms (shake effect)
```

---

## Smart Animate

**🔥 Feature más poderoso de Figma para prototipos**

### Qué es Smart Animate

Figma automáticamente anima las diferencias entre dos frames:
- Posición (X, Y)
- Tamaño (Width, Height)
- Rotación
- Opacidad
- Color
- Border radius
- Efectos

### Requisitos para que funcione

```
✓ Layers deben tener el MISMO NOMBRE en ambos frames
✓ Usar la misma estructura de capas
✓ Transition: Smart Animate
```

---

### Ejemplo 1: Card Expansion

**Frame 1: Card Collapsed**
```
Card (320px × 100px)
├── Image (80×80)
├── Title
└── Subtitle
```

**Frame 2: Card Expanded**
```
Card (320px × 400px) ← Mismo nombre!
├── Image (320×200) ← Mismo nombre!
├── Title ← Mismo nombre!
├── Subtitle ← Mismo nombre!
└── Description (nuevo elemento, fade in)
```

**Prototype:**
```
Card → On Click → Frame 2
Animation: Smart Animate
Duration: 400ms
Easing: Ease out
```

**Resultado:** Card se expande suavemente, imagen crece, descripción aparece

---

### Ejemplo 2: Morphing Shapes

```
Frame 1:
Rectangle "Shape" (100×100, blue, border-radius: 0)

Frame 2:
Rectangle "Shape" (100×100, red, border-radius: 50px)

Smart Animate:
- Color cambia gradualmente blue → red
- Esquinas se redondean 0 → 50px
```

---

### Ejemplo 3: Complex Animation

**Onboarding Screen Transition:**

```
Screen 1:
├── Illustration "Hero" (Y: 100)
├── Dot 1 (active)
├── Dot 2 (inactive)
├── Title (opacity: 1)
└── Next Button

Screen 2:
├── Illustration "Hero" (Y: 100) ← Misma posición
├── Dot 1 (inactive)
├── Dot 2 (active)
├── Title (opacity: 1, diferente texto)
└── Next Button

Smart Animate Result:
- Dots change state smoothly
- Title cross-fades
- Hero illustration stays (no animation)
```

---

## Prototipos para Testing

### Preparar Prototipo para Usability Testing

#### Checklist Pre-Test

```
✓ Todas las interacciones principales funcionan
✓ No hay "dead ends" (pantallas sin salida)
✓ Starting frame definido (marca frame como start)
✓ Flujos completos de principio a fin
✓ Estados de error incluidos
✓ Mensajes de feedback visibles
✓ No hay lorem ipsum en textos críticos
✓ Performance smooth (no lag)
```

#### Configurar Starting Point

```
1. Selecciona el frame inicial (Home o Onboarding)
2. Panel Prototype
3. Flow starting point → Marcar
4. Aparece ícono "play" azul en el frame
```

#### Crear Múltiples Flows

**Para testear diferentes user journeys:**

```
Flow 1: "New User"
Starting point: Onboarding Screen

Flow 2: "Returning User"
Starting point: Home Screen

Flow 3: "Error Scenario"
Starting point: Screen con error

En Share settings:
Show: All flows
User can switch flows
```

---

### Device Frames

**Hacer más realista:**

```
1. Selecciona frame
2. Panel derecho → Prototype
3. Device: iPhone 14 Pro
4. Show device frame: ✓
5. Color: Black / White / etc

Resultado: Prototipo se ve dentro de un iPhone real
```

---

## Ejercicios Prácticos

### 🎯 Ejercicio 1: Bottom Navigation (20 min)

**Objetivo:** Crear navegación entre 3 tabs

```
Crear 3 screens:
1. Home
2. Search
3. Profile

Bottom Nav en cada screen:
[🏠 Home] [🔍 Search] [👤 Profile]

Requisitos:
✓ Clicking cada icon navega a su screen
✓ Active state: Icon + text en primary color
✓ Inactive state: Icon + text en gray
✓ Transition: Instant (no animation entre tabs)
✓ Smart Animate para active indicator
```

---

### 🎯 Ejercicio 2: Login Flow (30 min)

**Objetivo:** Prototipo interactivo completo

```
Screens:
1. Login
2. Loading
3. Success → Home

Flow:
1. User ingresa email/password
2. Click "Login"
3. Button → Loading state (spinner)
4. After 2s → Success screen
5. After 1s → Navigate Home

Requisitos:
✓ Input focus states
✓ Button states (default, hover, loading)
✓ Success animation (checkmark)
✓ Smooth transitions
```

---

### 🎯 Ejercicio 3: Modal Overlay (15 min)

**Objetivo:** Confirmation dialog

```
Pantalla con button "Delete Account"

Al presionar:
- Overlay aparece (center)
- Background oscurecido
- Modal con:
  "Are you sure?"
  [Cancel] [Confirm]

Requisitos:
✓ Overlay: Dissolve animation
✓ Cancel: Close overlay
✓ Confirm: Navigate to success
✓ Click outside: Close overlay
```

---

### 🎯 Ejercicio 4: Card Interaction (25 min)

**Objetivo:** Product card expandible

```
Grid de Product Cards

Al click en card:
- Card expande full screen
- Image crece
- Más información aparece
- Add to Cart button

Requisitos:
✓ Smart Animate para expansion
✓ Back button funcional
✓ Add to Cart → Show confirmation
✓ Smooth all transitions
```

---

### 🎯 Ejercicio 5: Prototipo Completo (60 min)

**Objetivo:** E-commerce checkout flow

```
Screens:
1. Product List
2. Product Detail
3. Cart
4. Checkout (form)
5. Payment
6. Success

Requisitos:
✓ Navegación completa
✓ Add to cart animation
✓ Form validation states
✓ Loading state en payment
✓ Success celebration
✓ Todas micro-interactions
✓ Hover states
✓ Error scenarios
```

---

## Tips Pro para Prototipos

### 1. Naming Convention
```
✓ BIEN: "Button - Primary"
✗ MAL: "Rectangle 1"

Para Smart Animate:
✓ BIEN: Mismo nombre en ambos frames
✗ MAL: "Card" y "Card Copy"
```

### 2. Performance

```
✓ Usa components (más rápido)
✓ Limita shadows complejos
✓ Optimiza imágenes
✗ Evita demasiadas layers
✗ Evita efectos pesados en animaciones
```

### 3. Organización

```
Nombra frames claramente:
✓ "01 - Onboarding 1"
✓ "02 - Onboarding 2"
✓ "03 - Home"

Agrupa por flows:
✓ Frame "📱 Mobile Prototype"
  ├── Flow: Onboarding
  ├── Flow: Main App
  └── Flow: Settings
```

### 4. Documentación

```
Agrega notas con comentarios:
- "This animation needs refinement"
- "API loading takes 2-3s in reality"
- "Error state not yet designed"

Usa Sticky Notes en Figma
```

---

## Recursos Adicionales

### Plugins Útiles para Prototipos
- **Figmotion**: Animaciones complejas
- **Autoflow**: Generar flowcharts automáticos
- **Stark**: Verificar accesibilidad
- **Similayer**: Copiar estilos entre layers

### Inspiración
- **Mobbin**: Prototipos móviles reales
- **Dribbble**: Micro-interactions
- **UI Movement**: Animaciones inspiradoras

### Tutoriales Avanzados
- Figma YouTube Channel
- DesignCourse
- Flux Academy

---

## Checklist Final

Antes de compartir tu prototipo:

```
[ ] Todas las interacciones funcionan
[ ] No hay dead ends
[ ] Starting frame definido
[ ] Transiciones suaves
[ ] Loading states incluidos
[ ] Error states considerados
[ ] Performance optimizado
[ ] Tested en mobile (si aplica)
[ ] Comments/notas agregados
[ ] Link de share configurado correctamente
```

---

**¡Listo para crear prototipos profesionales! 🚀**