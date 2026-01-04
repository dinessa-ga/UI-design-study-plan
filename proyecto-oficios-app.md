# Proyecto Completo: "OficiosConnect"
## Marketplace de Servicios y Capacitaciones para Oficios

---

## 📋 Índice
1. [Brief del Proyecto](#brief-del-proyecto)
2. [Research & Discovery](#research--discovery)
3. [Define](#define)
4. [User Flows](#user-flows)
5. [Arquitectura de Información](#arquitectura-de-información)
6. [Wireframes](#wireframes)
7. [Design System](#design-system)
8. [Pantallas Completas (Mockups)](#pantallas-completas)
9. [Prototipo Interactivo](#prototipo-interactivo)
10. [Micro-interactions](#micro-interactions)
11. [Testing Plan](#testing-plan)

---

## Brief del Proyecto

### 🎯 Objetivo
Crear una plataforma móvil que conecte profesionales de oficios con clientes que necesitan servicios O quieren aprender el oficio.

### 👥 Usuarios Principales

**Tipo A: Clientes/Estudiantes**
- Necesitan contratar servicios (reparar algo, construir, arreglar)
- Quieren aprender un oficio nuevo
- Edades: 25-55 años
- Tech-savvy: Medio

**Tipo B: Profesionales de Oficios**
- Carpinteros, electricistas, plomeros, mecánicos
- Peluqueros, reposteros, costureras
- Técnicos (celulares, PCs, electrodomésticos)
- Quieren conseguir más clientes
- Pueden ofrecer capacitaciones
- Edades: 30-60 años
- Tech-savvy: Bajo-Medio

### 💡 Propuesta de Valor

**Para Clientes:**
- Encontrar profesionales confiables cerca de ti
- Ver trabajos previos y reviews
- Reservar servicios fácilmente
- Aprender oficios directamente de expertos

**Para Profesionales:**
- Conseguir más clientes
- Monetizar su conocimiento con cursos
- Construir reputación online
- Gestionar agenda

### 🏆 Competencia
- **TaskRabbit**: Servicios generales (muy amplio, poco especializado)
- **Thumbtack**: Profesionales locales (USA, interface compleja)
- **YouTube/Udemy**: Cursos online (no servicios locales)
- **Mercado Libre Servicios**: Marketplace genérico (poca confianza)

### 🎨 Diferenciadores
1. **Híbrido**: Servicios + Educación en misma plataforma
2. **Local-first**: Enfocado en tu zona/ciudad
3. **Portfolio visual**: Galería de trabajos anteriores
4. **Verificación**: Profesionales verificados
5. **Comunidad**: Reviews bidireccionales y reputación

---

## Research & Discovery

### 🔍 User Research Summary

#### Entrevistas (5 clientes, 5 profesionales)

**Insights de Clientes:**
```
Pain Points:
❌ "No sé si el profesional es confiable"
❌ "No tengo idea de precios justos"
❌ "Difícil comparar opciones"
❌ "Miedo a que no lleguen o hagan mal trabajo"

Necesidades:
✓ Ver trabajos anteriores
✓ Reviews de otros clientes
✓ Precio estimado antes de contratar
✓ Comunicación directa
✓ Garantía de servicio
```

**Insights de Profesionales:**
```
Pain Points:
❌ "Dependo del boca a boca"
❌ "Clientes preguntan pero no contratan"
❌ "Difícil mostrar mi trabajo"
❌ "Competencia desleal (precios muy bajos)"

Necesidades:
✓ Mostrar portfolio fácilmente
✓ Gestionar agenda
✓ Cobrar anticipos
✓ Construir reputación
✓ Ingreso extra con cursos
```

### 📊 User Personas

#### Persona 1: Cliente/Estudiante

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[Foto: Hombre 35 años]

CARLOS MENDOZA
35 años | Ingeniero de Software | Guayaquil

DEMOGRAFÍA:
• Casado, 1 hijo
• Ingresos: $1,800/mes
• Vive en casa propia
• Usa: iPhone, laptop

OBJETIVOS:
1. Encontrar carpintero para closet
2. Reparar laptop de forma rápida
3. Aprender plomería básica para su casa

FRUSTRACIONES:
1. No sabe a quién llamar cuando algo se daña
2. Miedo a que le cobren de más
3. Ha tenido malas experiencias (no llegan)
4. Pierde tiempo buscando en grupos de Facebook

COMPORTAMIENTO:
"Cuando necesito algo, pregunto en grupos de WhatsApp 
de mi residencial. A veces encuentro, a veces no. 
Me gustaría ver trabajos anteriores antes de decidir."

QUOTE:
"Solo quiero saber que la persona es buena y confiable 
antes de darle mi dinero"

TECH LEVEL: █████░ (5/6)
URGENCIA: ████░░ (4/6) - Necesita soluciones rápidas
PRESUPUESTO: ████░░ (4/6) - Dispuesto a pagar precio justo
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

#### Persona 2: Profesional

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
[Foto: Hombre 42 años]

JOSÉ RAMÍREZ
42 años | Carpintero | Guayaquil
20 años de experiencia

DEMOGRAFÍA:
• Casado, 3 hijos
• Ingresos variables: $800-1,500/mes
• Negocio independiente
• Usa: Android, WhatsApp principalmente

OBJETIVOS:
1. Conseguir más clientes constantes
2. Mostrar su trabajo (hace muebles hermosos)
3. Dar clases de carpintería básica (fin de semana)
4. Dejar de depender solo de referencias

FRUSTRACIONES:
1. Clientes piden presupuesto y desaparecen
2. No tiene forma de mostrar trabajos anteriores profesionalmente
3. Competencia con precios muy bajos (mala calidad)
4. Difícil llenar agenda completa

COMPORTAMIENTO:
"Tengo fotos de mis trabajos en mi galería pero no sé 
cómo mostrarlas bien. Los clientes me encuentran por 
referencias de otros clientes o en grupos de Facebook."

QUOTE:
"Si pudiera mostrar todo lo que he hecho, la gente 
vería que valgo lo que cobro"

TECH LEVEL: ███░░░ (3/6)
MOTIVACIÓN DIGITAL: █████░ (5/6) - Quiere crecer
DISPONIBILIDAD: ████░░ (4/6) - Quiere más trabajo
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## Define

### 🎯 Problem Statements

**Para Clientes:**
```
Carlos necesita encontrar profesionales confiables 
de forma rápida y segura porque las opciones actuales 
(grupos de WhatsApp/Facebook) no le dan garantías 
sobre la calidad del trabajo y teme perder su dinero.
```

**Para Profesionales:**
```
José necesita mostrar su trabajo profesionalmente 
y conseguir clientes constantes porque depende solo 
de referencias y no tiene forma de competir visualmente 
con su experiencia y calidad de trabajo.
```

### 💭 How Might We Questions

```
🤔 HMW generar confianza entre clientes y profesionales?
🤔 HMW hacer que profesionales muestren su trabajo fácilmente?
🤔 HMW reducir el miedo a contratar alguien desconocido?
🤔 HMW ayudar a profesionales a monetizar su conocimiento?
🤔 HMW simplificar la búsqueda y comparación?
🤔 HMW garantizar que ambas partes cumplan compromisos?
🤔 HMW hacer que profesionales poco tech-savvy usen la app?
```

### ✨ Key Features (MVP)

#### Para Clientes
```
✓ Búsqueda por oficio + ubicación
✓ Ver portfolio de trabajos (fotos/videos)
✓ Reviews y ratings
✓ Solicitar cotización
✓ Chat directo con profesional
✓ Reservar servicio
✓ Buscar y comprar cursos/talleres
```

#### Para Profesionales
```
✓ Crear perfil con portfolio
✓ Subir fotos/videos de trabajos
✓ Recibir solicitudes de cotización
✓ Chat con clientes
✓ Gestionar agenda
✓ Publicar cursos/talleres
✓ Recibir pagos
```

---

## User Flows

### Flow 1: Cliente busca y contrata servicio

```
┌─────────────────────────────────────────────────────────┐
│                    FLOW: CONTRATAR SERVICIO             │
└─────────────────────────────────────────────────────────┘

1. INICIO
   │
   ├─→ Usuario nuevo → Onboarding (3 screens)
   │                    └─→ Registro rápido
   │
   └─→ Usuario returning → Skip to Home
   │
   ↓
2. HOME
   │
   ├─→ Búsqueda por categoría (ej: "Carpintería")
   │   O
   └─→ Búsqueda por keyword (ej: "reparar closet")
   │
   ↓
3. SEARCH RESULTS
   │
   Muestra lista de profesionales:
   ├─→ Filtros (precio, distancia, rating)
   ├─→ Ordenar (mejor valorados, cerca, precio)
   │
   Usuario selecciona uno →
   │
   ↓
4. PERFIL PROFESIONAL
   │
   Ve:
   ├─→ Portfolio (fotos de trabajos)
   ├─→ Reviews
   ├─→ Servicios que ofrece
   ├─→ Precios aproximados
   │
   Decisión:
   ├─→ Ver cursos de este profesional
   ├─→ Solicitar cotización
   └─→ Reservar directo (si tiene slots)
   │
   ↓
5. SOLICITAR COTIZACIÓN
   │
   ├─→ Describe el trabajo (texto + fotos)
   ├─→ Selecciona fecha preferida
   ├─→ Envía solicitud
   │
   ↓
6. ESPERA RESPUESTA
   │
   Profesional responde con:
   ├─→ Precio estimado
   ├─→ Tiempo estimado
   └─→ Disponibilidad
   │
   ↓
7. CONFIRMAR RESERVA
   │
   ├─→ Acepta cotización
   ├─→ Paga anticipo (opcional, 30%)
   └─→ Confirma fecha/hora
   │
   ↓
8. CONFIRMACIÓN
   │
   ├─→ Detalles del servicio
   ├─→ Info de contacto profesional
   ├─→ Agregar a calendario
   └─→ Chat disponible
   │
   ↓
9. DÍA DEL SERVICIO
   │
   ├─→ Recordatorio 24h antes
   ├─→ Recordatorio 2h antes
   └─→ Tracking (profesional en camino)
   │
   ↓
10. POST-SERVICIO
    │
    ├─→ Pago restante
    ├─→ Dejar review y rating
    └─→ Guardar en favoritos
    │
    ✓ FIN
```

### Flow 2: Profesional recibe y acepta trabajo

```
┌─────────────────────────────────────────────────────────┐
│                FLOW: PROFESIONAL RECIBE TRABAJO         │
└─────────────────────────────────────────────────────────┘

1. NOTIFICACIÓN
   │
   "Nueva solicitud de cotización"
   │
   ↓
2. VER SOLICITUD
   │
   Muestra:
   ├─→ Info del cliente (nombre, ubicación)
   ├─→ Descripción del trabajo
   ├─→ Fotos (si adjuntó)
   └─→ Fecha preferida
   │
   Opciones:
   ├─→ Rechazar (con motivo)
   └─→ Responder con cotización
   │
   ↓
3. CREAR COTIZACIÓN
   │
   ├─→ Precio (input)
   ├─→ Tiempo estimado
   ├─→ Disponibilidad (seleccionar slots)
   ├─→ Notas adicionales
   └─→ Enviar
   │
   ↓
4. ESPERA CONFIRMACIÓN
   │
   Cliente acepta →
   │
   ↓
5. TRABAJO CONFIRMADO
   │
   ├─→ Ver detalles completos
   ├─→ Ubicación en mapa
   ├─→ Chat con cliente
   └─→ Agregar a agenda
   │
   ↓
6. DÍA DEL SERVICIO
   │
   ├─→ Ver trabajos del día
   ├─→ Notificación 2h antes
   ├─→ Activar "En camino" (tracking)
   └─→ Llegó → Marcar "Trabajando"
   │
   ↓
7. FINALIZAR TRABAJO
   │
   ├─→ Subir fotos del trabajo terminado
   ├─→ Marcar como "Completado"
   ├─→ Solicitar pago restante
   └─→ Invitar a dejar review
   │
   ✓ FIN
```

### Flow 3: Cliente busca y compra curso

```
┌─────────────────────────────────────────────────────────┐
│                  FLOW: COMPRAR CURSO                    │
└─────────────────────────────────────────────────────────┘

1. HOME
   │
   ├─→ Tab "Servicios"
   └─→ Tab "Cursos" ←
   │
   ↓
2. EXPLORAR CURSOS
   │
   Categorías:
   ├─→ Carpintería
   ├─→ Electricidad
   ├─→ Plomería
   ├─→ Mecánica
   └─→ Más...
   │
   O Búsqueda directa
   │
   ↓
3. LISTA DE CURSOS
   │
   Cards muestran:
   ├─→ Título del curso
   ├─→ Instructor (con rating)
   ├─→ Duración (ej: 4 sesiones)
   ├─→ Precio
   ├─→ Modalidad (presencial/online)
   └─→ Próxima fecha
   │
   Usuario selecciona →
   │
   ↓
4. DETALLE DEL CURSO
   │
   ├─→ Descripción completa
   ├─→ Qué aprenderás
   ├─→ Requisitos
   ├─→ Cronograma
   ├─→ Perfil del instructor
   ├─→ Reviews de estudiantes previos
   │
   Opciones:
   ├─→ Ver perfil del instructor
   └─→ Inscribirse
   │
   ↓
5. INSCRIPCIÓN
   │
   ├─→ Seleccionar fecha/horario
   ├─→ Confirmar datos
   ├─→ Pago completo
   └─→ Confirmar
   │
   ↓
6. CONFIRMACIÓN
   │
   ├─→ Detalles del curso
   ├─→ Link de Zoom (si online)
   ├─→ Ubicación (si presencial)
   ├─→ Agregar a calendario
   └─→ Chat con instructor
   │
   ↓
7. RECORDATORIOS
   │
   ├─→ 1 semana antes: "Tu curso inicia pronto"
   ├─→ 1 día antes: Recordatorio + preparativos
   └─→ 1 hora antes: "Tu clase empieza en 1h"
   │
   ✓ FIN
```

---

## Arquitectura de Información

### Estructura de Navegación (Bottom Tabs)

```
┌─────────────────────────────────────────────────────┐
│                                                     │
│                   [Content Area]                    │
│                                                     │
│                                                     │
├─────────────────────────────────────────────────────┤
│  [🏠]      [🔍]      [💼]      [💬]      [👤]     │
│  Home    Explorar   Trabajos   Chat    Perfil      │
└─────────────────────────────────────────────────────┘

HOME:
├── Búsqueda rápida
├── Categorías populares
├── Servicios cercanos destacados
├── Cursos recomendados
└── Banners promocionales

EXPLORAR:
├── Tab: Servicios
│   ├── Búsqueda avanzada
│   ├── Filtros
│   └── Resultados
└── Tab: Cursos
    ├── Categorías
    ├── Filtros
    └── Resultados

TRABAJOS (contexto según rol):
├── Cliente:
│   ├── Activos (en progreso)
│   ├── Pendientes (cotizaciones)
│   └── Historial (completados)
│
└── Profesional:
    ├── Solicitudes nuevas
    ├── Confirmados
    ├── En progreso
    └── Completados

CHAT:
├── Conversaciones activas
├── Archivadas
└── Notificaciones

PERFIL:
├── Mi información
├── Mi portfolio (si profesional)
├── Mis cursos (si profesional)
├── Favoritos
├── Reviews recibidas
├── Configuración
└── Ayuda
```

### Onboarding (Primera vez)

```
Screen 1: Welcome
├── Ilustración
├── "Conecta con expertos en oficios"
└── [Continuar]

Screen 2: Rol Selection
├── "¿Cómo quieres usar OficiosConnect?"
├── [Busco servicios/cursos] (Cliente)
├── [Ofrezco servicios/cursos] (Profesional)
└── Nota: "Puedes cambiar después"

Screen 3: Ubicación
├── "¿Dónde estás ubicado?"
├── [Permitir ubicación]
└── O ingreso manual de ciudad

Screen 4: Intereses (depende del rol)
│
├→ Cliente: Categorías de interés
│  ├── Carpintería
│  ├── Electricidad
│  └── Plomería (selección múltiple)
│
└→ Profesional: Tu especialidad
   └── Selecciona tu oficio principal

Screen 5: Registro
├── Email/Password
├── O continuar con Google
└── [Crear cuenta]

→ HOME
```

---

## Wireframes

### Home Screen (Cliente)

```
┌─────────────────────────────────────────┐
│ 9:41        OficiosConnect     🔔  ⚙️   │ ← Status + Header
├─────────────────────────────────────────┤
│                                         │
│ Hola, Carlos 👋                         │ ← Saludo personalizado
│ ¿Qué necesitas hoy?                     │
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │  🔍 Buscar servicios o cursos...    │ │ ← Search bar
│ └─────────────────────────────────────┘ │
│                                         │
│ Categorías populares:                   │ ← Quick access
│                                         │
│ [🔨]   [⚡]   [🔧]   [💇]   [🍰]       │
│ Carpin Electri Plome Pelu  Paste       │
│                                         │
│ [Ver todas →]                           │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Cerca de ti:                            │ ← Geolocation-based
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ [IMG]  José Ramírez                 │ │
│ │        Carpintero                   │ │
│ │        ⭐ 4.9 (127)  📍 2.3 km      │ │
│ │        [Ver perfil →]               │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ [IMG]  María López                  │ │
│ │        Electricista                 │ │
│ │        ⭐ 4.8 (89)   📍 3.1 km      │ │
│ │        [Ver perfil →]               │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Cursos recomendados:                    │ ← Personalized
│                                         │
│ ┌──────────┬──────────┬──────────┐     │
│ │[IMG]     │[IMG]     │[IMG]     │     │
│ │Carpinte  │Electrici │Plomería  │     │
│ │básica    │domicilio │básica    │     │
│ │$80 4sem  │$60 3sem  │$50 2sem  │     │
│ └──────────┴──────────┴──────────┘     │
│                                         │
│ [Ver más cursos →]                      │
│                                         │
├─────────────────────────────────────────┤
│ [🏠]  [🔍]  [💼]  [💬]  [👤]           │ ← Bottom Nav
│ Home  Buscar Trabajos Chat  Perfil     │
└─────────────────────────────────────────┘
```

### Search Results Screen

```
┌─────────────────────────────────────────┐
│ ←  Carpinteros                    🔍    │ ← Back + Search again
├─────────────────────────────────────────┤
│                                         │
│ 📍 Guayaquil [Cambiar]                  │ ← Location
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ Filtros: [Distancia ▼][Precio ▼]   │ │ ← Filters
│ │ Ordenar: [Mejor valorados ▼]        │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ 24 profesionales encontrados            │
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ [Foto]  José Ramírez            ⭐  │ │ ← Card
│ │         Carpintero                  │ │
│ │         ⭐ 4.9 (127 reviews)         │ │
│ │         📍 2.3 km • Urdesa          │ │
│ │         💰 Desde $40/hora           │ │
│ │         ✅ Verificado               │ │
│ │                                     │ │
│ │         "Muebles a medida..."       │ │ ← Bio preview
│ │                                     │ │
│ │         [Ver perfil] [Cotizar]      │ │ ← CTAs
│ └─────────────────────────────────────┘ │
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ [Foto]  Carlos Vera             ⭐  │ │
│ │         Carpintero                  │ │
│ │         ⭐ 4.7 (45 reviews)          │ │
│ │         📍 4.1 km • Samborondón     │ │
│ │         💰 Desde $35/hora           │ │
│ │                                     │ │
│ │         "Especialista en..."        │ │
│ │                                     │ │
│ │         [Ver perfil] [Cotizar]      │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ [Cargar más...]                         │
│                                         │
├─────────────────────────────────────────┤
│ [🏠]  [🔍]  [💼]  [💬]  [👤]           │
└─────────────────────────────────────────┘
```

### Professional Profile Screen

```
┌─────────────────────────────────────────┐
│ ←                            ⋮ ❤️       │ ← Back, Menu, Favorite
├─────────────────────────────────────────┤
│                                         │
│        [Foto Perfil Grande]             │ ← Hero
│                                         │
│         José Ramírez                    │ ← Name
│         Carpintero ✅                   │ ← Trade + Verified
│         ⭐ 4.9 (127)  📍 2.3 km         │ ← Stats
│                                         │
│ [💬 Chat]  [📞 Llamar]  [Cotizar]      │ ← Quick actions
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Tabs: [Portfolio] Servicios Reviews     │ ← Tabs navigation
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ TAB: PORTFOLIO                      │ │
│ ├─────────────────────────────────────┤ │
│ │                                     │ │
│ │ Grid de fotos (3 columnas):         │ │
│ │                                     │ │
│ │ [IMG] [IMG] [IMG]                   │ │
│ │ [IMG] [IMG] [IMG]                   │ │
│ │ [IMG] [IMG] [IMG]                   │ │
│ │                                     │ │
│ │ Cada foto clickeable para ver       │ │
│ │ detalle + descripción               │ │
│ │                                     │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ Sobre mí:                               │
│ "Carpintero con 20 años de experiencia  │
│ en muebles a medida, cocinas integrales │
│ y restauración de muebles antiguos..."  │
│                                         │
│ Especialidades:                         │
│ • Muebles a medida                      │
│ • Cocinas integrales                    │
│ • Closets                               │
│ • Restauración                          │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Cursos que ofrece:                      │ ← Cross-sell
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ [IMG] Carpintería Básica            │ │
│ │       4 sesiones • $80              │ │
│ │       [Ver curso →]                 │ │
│ └─────────────────────────────────────┘ │
│                                         │
├─────────────────────────────────────────┤
│ [🏠]  [🔍]  [💼]  [💬]  [👤]           │
└─────────────────────────────────────────┘
```

### Request Quote Screen

```
┌─────────────────────────────────────────┐
│ ←  Solicitar Cotización                 │
├─────────────────────────────────────────┤
│                                         │
│ Para: José Ramírez                      │ ← Professional
│ Servicio: Carpintería                   │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Describe el trabajo:                    │
│ ┌─────────────────────────────────────┐ │
│ │ Necesito hacer un closet            │ │ ← Text area
│ │ para mi habitación de                │ │
│ │ aproximadamente 2m x 2.5m...         │ │
│ │                                     │ │
│ └─────────────────────────────────────┘ │
│ 250/500 caracteres                      │
│                                         │
│ Agregar fotos (opcional):               │
│ [📷] [📷] [📷]                          │ ← Photo upload
│  +    +    +                            │
│                                         │
│ ¿Cuándo lo necesitas?                   │
│ ┌─────────────────────────────────────┐ │
│ │ 📅 [Seleccionar fecha]              │ │ ← Date picker
│ └─────────────────────────────────────┘ │
│                                         │
│ ○ Lo antes posible                      │ ← Radio options
│ ○ Fecha específica                      │
│ ○ Flexible                              │
│                                         │
│ Ubicación:                              │
│ 📍 Av. Principal 123, Urdesa            │ ← Auto from profile
│ [Cambiar ubicación]                     │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Presupuesto aproximado:                 │
│ ┌─────────────────────────────────────┐ │
│ │ $ [___________]                     │ │ ← Input
│ └─────────────────────────────────────┘ │
│ (Opcional - ayuda al profesional)       │
│                                         │
│                                         │
│ [Enviar solicitud]                      │ ← Primary CTA
│                                         │
├─────────────────────────────────────────┤
│ [🏠]  [🔍]  [💼]  [💬]  [👤]           │
└─────────────────────────────────────────┘
```

### Quote Received (Professional Side)

```
┌─────────────────────────────────────────┐
│ ←  Solicitud de Cotización              │
├─────────────────────────────────────────┤
│                                         │
│ De: Carlos Mendoza                      │ ← Client
│ ⭐ Cliente verificado                   │
│ 📍 2.3 km de distancia                  │
│ 🕐 Recibido: Hace 2 horas               │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Descripción del trabajo:                │
│                                         │
│ "Necesito hacer un closet para mi       │
│ habitación de aproximadamente            │
│ 2m x 2.5m. Tengo el espacio listo..."   │
│                                         │
│ Fotos adjuntas:                         │
│ [IMG] [IMG] [IMG]                       │ ← Gallery
│                                         │
│ Fecha solicitada:                       │
│ 📅 15 de Enero (Flexible)               │
│                                         │
│ Presupuesto del cliente:                │
│ 💰 $500 - $800                          │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Tu respuesta:                           │
│                                         │
│ Precio:                                 │
│ ┌─────────────────────────────────────┐ │
│ │ $ [___________]                     │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ Tiempo estimado:                        │
│ ┌─────────────────────────────────────┐ │
│ │ [__] días                           │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ Tu disponibilidad:                      │
│ ┌─────────────────────────────────────┐ │
│ │ 📅 [Seleccionar fechas]             │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ Notas adicionales:                      │
│ ┌─────────────────────────────────────┐ │
│ │ (Opcional - materiales, proceso,    │ │
│ │  etc)                               │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ [Rechazar]          [Enviar cotización] │
│                                         │
├─────────────────────────────────────────┤
│ [🏠]  [🔍]  [💼]  [💬]  [👤]           │
└─────────────────────────────────────────┘
```

### Course Detail Screen

```
┌─────────────────────────────────────────┐
│ ←                            ⋮ ❤️       │
├─────────────────────────────────────────┤
│                                         │
│      [Imagen Cover del Curso]           │ ← Hero image
│                                         │
├─────────────────────────────────────────┤
│                                         │
│ Carpintería Básica                      │ ← Title H1
│ para principiantes                      │
│                                         │
│ [Foto] José Ramírez                     │ ← Instructor
│        ⭐ 4.9 (127 reviews)             │
│        [Ver perfil →]                   │
│                                         │
│ 💰 $80    ⏱ 4 sesiones    👥 8 cupos   │ ← Quick stats
│                                         │
│ 📅 Próxima fecha: Sábado 20 Enero       │
│ 🕐 9:00 AM - 12:00 PM                   │
│ 📍 Taller del instructor (Urdesa)       │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Tabs: [Descripción] Temario Reviews     │
│                                         │
│ ¿Qué aprenderás?                        │
│                                         │
│ ✓ Uso seguro de herramientas básicas    │
│ ✓ Técnicas de corte y ensamblaje       │
│ ✓ Acabados y lijado                     │
│ ✓ Proyecto final: mesa pequeña          │
│                                         │
│ Descripción:                            │
│ "Curso introductorio de carpintería     │
│ donde aprenderás las bases necesarias    │
│ para comenzar tus propios proyectos..."  │
│                                         │
│ Requisitos:                             │
│ • Ninguno - apto para principiantes     │
│ • Traer ropa cómoda que pueda ensuciarse│
│ • Ganas de aprender                     │
│                                         │
│ Incluye:                                │
│ ✓ Materiales para el proyecto           │
│ ✓ Uso de herramientas del taller        │
│ ✓ Manual digital del curso              │
│ ✓ Certificado de participación          │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ [Inscribirme - $80]                     │ ← Sticky CTA
│                                         │
├─────────────────────────────────────────┤
│ [🏠]  [🔍]  [💼]  [💬]  [👤]           │
└─────────────────────────────────────────┘
```

---

## Design System

### 🎨 Colors

```
PRIMARY (Blue):
- Primary-900: #1E3A8A (dark)
- Primary-700: #1D4ED8
- Primary-500: #3B82F6 (main)
- Primary-300: #93C5FD
- Primary-100: #DBEAFE (backgrounds)

SECONDARY (Orange - warmth/craft):
- Secondary-500: #F59E0B (accents)
- Secondary-300: #FCD34D
- Secondary-100: #FEF3C7

SUCCESS:
- Success-500: #10B981 (verified, completed)
- Success-100: #D1FAE5

ERROR:
- Error-500: #EF4444 (alerts, cancelled)
- Error-100: #FEE2E2

WARNING:
- Warning-500: #F59E0B (pending)
- Warning-100: #FEF3C7

NEUTRAL (Grays):
- N-900: #111827 (main text)
- N-700: #374151 (secondary text)
- N-500: #6B7280 (placeholder)
- N-300: #D1D5DB (borders)
- N-100: #F3F4F6 (light backgrounds)
- N-50: #F9FAFB (cards)
- White: #FFFFFF

GRADIENT (Hero sections):
linear-gradient(135deg, #3B82F6 0%, #1D4ED8 100%)
```

### 📝 Typography

```
FONT FAMILY: Inter (Google Fonts)

SCALE:

Display:
- Size: 32px
- Weight: Bold (700)
- Line-height: 40px
- Use: Onboarding titles, hero

H1:
- Size: 28px
- Weight: Bold (700)
- Line-height: 36px
- Use: Page titles

H2:
- Size: 20px
- Weight: Semibold (600)
- Line-height: 28px
- Use: Section titles, card titles

H3:
- Size: 18px
- Weight: Semibold (600)
- Line-height: 24px
- Use: Subsections

Body Large:
- Size: 16px
- Weight: Regular (400)
- Line-height: 24px
- Use: Main content

Body:
- Size: 14px
- Weight: Regular (400)
- Line-height: 20px
- Use: Descriptions, secondary info

Caption:
- Size: 12px
- Weight: Regular (400)
- Line-height: 16px
- Use: Labels, metadata

Button Text:
- Size: 16px
- Weight: Semibold (600)
- Line-height: 24px
```

### 🔘 Components

#### Button System

```
PRIMARY BUTTON:
- Background: Primary-500
- Text: White
- Padding: 16px horizontal, 14px vertical
- Border-radius: 12px
- Font: 16px Semibold
- Shadow: 0 2px 8px rgba(59,130,246,0.2)

States:
- Hover: Primary-600 + scale(1.02)
- Pressed: Primary-700 + scale(0.98)
- Disabled: N-300 bg, N-500 text
- Loading: Spinner + Primary-500 bg

SECONDARY BUTTON:
- Background: White
- Text: Primary-500
- Border: 2px solid Primary-500
- Padding: 14px horizontal, 12px vertical
- Border-radius: 12px

GHOST BUTTON:
- Background: Transparent
- Text: Primary-500
- No border
- Hover: Primary-100 background

ICON BUTTON:
- Size: 44×44 (touch target)
- Icon: 24×24
- Border-radius: 12px
- Hover: N-100 background
```

#### Card Component

```
STANDARD CARD:
- Background: White
- Padding: 16px
- Border-radius: 16px
- Shadow: 0 2px 12px rgba(0,0,0,0.08)
- Border: 1px solid N-200 (optional)

PROFESSIONAL CARD:
┌─────────────────────────────┐
│ [Avatar]  Name           ⭐ │
│           Trade             │
│           ⭐ X.X (N)  📍 Xkm│
│           💰 Desde $XX      │
│           [CTA] [CTA]       │
└─────────────────────────────┘
- Height: Hug content
- Hover: Shadow increases, slight scale(1.02)

COURSE CARD:
┌─────────────────┐
│ [Cover Image]   │
│ Title           │
│ Instructor      │
│ $XX • X sesiones│
│ ⭐ X.X (N)      │
└─────────────────┘
- Width: 160px
- Border-radius: 12px
- Shadow on hover
```

#### Input Fields

```
TEXT INPUT:
- Height: 48px
- Padding: 12px 16px
- Border: 1px solid N-300
- Border-radius: 12px
- Font: 16px Regular
- Placeholder: N-500

States:
- Default: N-300 border
- Focus: Primary-500 border (2px)
         + 0 0 0 4px rgba(59,130,246,0.1) shadow
- Error: Error-500 border (2px)
         + Error message below
- Disabled: N-100 background, N-400 text

TEXT AREA:
- Min-height: 120px
- Same styling as input
- Resize: vertical

LABEL:
- Font: 14px Medium
- Color: N-700
- Margin-bottom: 8px
```

#### Chips/Tags

```
CATEGORY CHIP:
- Padding: 8px 16px
- Border-radius: 20px (pill)
- Background: N-100
- Text: N-700, 14px Medium

Active state:
- Background: Primary-500
- Text: White

BADGE (verification, status):
- Padding: 4px 8px
- Border-radius: 6px
- Font: 12px Semibold
- Background varies by type:
  • Verified: Success-100, Success-700 text
  • Premium: Secondary-100, Secondary-700 text
  • New: Primary-100, Primary-700 text
```

### 📐 Spacing System (8pt Grid)

```
4px  - Minimal spacing (between icon and text)
8px  - Tight spacing (list items)
12px - Default spacing (card internal)
16px - Standard spacing (sections)
24px - Medium spacing (between components)
32px - Large spacing (major sections)
48px - XL spacing (hero sections)
64px - XXL spacing (page sections)
```

### 🖼 Iconography

```
ICON LIBRARY: Lucide Icons (React)

SIZES:
- 16px: Inline with small text
- 20px: Inline with body text
- 24px: Standard (buttons, navigation)
- 32px: Large (feature icons)
- 48px: Extra large (empty states)

STYLE: Outline (2px stroke)
COLOR: Inherits from text or N-700

COMMON ICONS:
🏠 Home
🔍 Search
💼 Briefcase (jobs/work)
💬 Message
👤 User
📍 Map Pin
⭐ Star
📅 Calendar
🕐 Clock
💰 Dollar Sign
📷 Camera
✓ Check
× X (close)
⚙️ Settings
```

### 🎭 Illustrations & Images

```
STYLE: Flat, modern, friendly
COLORS: Match brand palette

USAGE:
- Onboarding: Full-screen illustrations
- Empty states: Medium illustrations (200×200)
- Hero sections: Abstract shapes/patterns
- Professional photos: Real, authentic work photos

IMAGE SPECIFICATIONS:
- Profile photos: 1:1 ratio, min 400×400
- Portfolio photos: 4:3 ratio, min 800×600
- Course covers: 16:9 ratio, min 1200×675
- Compression: WebP format preferred
```

---

## Pantallas Completas (Mockups)

### 1. Onboarding Screen 1

```
┌─────────────────────────────────────────┐
│                                         │
│                                         │
│                                         │
│        [Ilustración Grande]             │
│     (Profesionales trabajando)          │
│                                         │
│                                         │
│                                         │
│         OficiosConnect                  │ ← Logo + Brand
│                                         │
│      Conecta con expertos               │ ← H1
│      en oficios locales                 │
│                                         │
│   Encuentra profesionales confiables     │ ← Body
│   o aprende nuevas habilidades          │
│                                         │
│   • • • ○                               │ ← Progress dots
│                                         │
│                                         │
│   [Continuar]                           │ ← Primary button
│                                         │
│   ¿Ya tienes cuenta? [Inicia sesión]   │ ← Link
│                                         │
└─────────────────────────────────────────┘

DESIGN DETAILS:
- Background: Gradient (Primary-500 to Primary-700)
- Illustration: Colorful, showing diversity of trades
- Text: White
- Button: White background, Primary-500 text
- Progress dots: White, semi-transparent
```

### 2. Home Screen (High Fidelity)

```
┌─────────────────────────────────────────┐
│ 9:41               🔔 ⚙️                │
├─────────────────────────────────────────┤
│                                         │
│ Hola, Carlos 👋                         │
│ ¿Qué necesitas hoy?                     │
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ 🔍  Buscar servicios o cursos...    │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ Categorías:                             │
│                                         │
│ ┌────┬────┬────┬────┬────┐            │
│ │[🔨]│[⚡]│[🔧]│[💇]│[🍰]│            │
│ │Carp│Elec│Plom│Pelu│Past│            │
│ └────┴────┴────┴────┴────┘            │
│                                         │
│ [Ver todas las categorías →]            │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Profesionales cerca de ti:              │
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ ┌────┐                              │ │
│ │ │IMG │ José Ramírez            ❤️   │ │
│ │ └────┘ Carpintero                   │ │
│ │        ⭐ 4.9 • 127 reviews         │ │
│ │        📍 2.3 km • Urdesa           │ │
│ │        💰 $40-60/hora               │ │
│ │        ✅ Verificado                │ │
│ │                                     │ │
│ │        [Ver perfil]    [Cotizar]    │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ ┌────┐                              │ │
│ │ │IMG │ María López             ❤️   │ │
│ │ └────┘ Electricista                 │ │
│ │        ⭐ 4.8 • 89 reviews          │ │
│ │        📍 3.1 km • Samborondón      │ │
│ │        💰 $35-50/hora               │ │
│ │                                     │ │
│ │        [Ver perfil]    [Cotizar]    │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Cursos populares:                       │
│                                         │
│ ┌────────┬────────┬────────┐           │
│ │ [IMG]  │ [IMG]  │ [IMG]  │           │
│ │        │        │        │           │
│ │Carpint │Electri │Plomería│           │
│ │básica  │domicil │básica  │           │
│ │        │        │        │           │
│ │$80     │$60     │$50     │           │
│ │⭐ 4.9  │⭐ 4.7  │⭐ 4.8  │           │
│ └────────┴────────┴────────┘           │
│                                         │
│ [Ver todos los cursos →]                │
│                                         │
├─────────────────────────────────────────┤
│  [🏠]     [🔍]     [💼]     [💬]  [👤] │
│  Home   Explorar Trabajos  Chat  Perfil│
└─────────────────────────────────────────┘

COLORS:
- Background: N-50 (#F9FAFB)
- Cards: White with shadow
- Primary text: N-900
- Secondary text: N-600
- Icons: Primary-500
- Active tab: Primary-500
```

### 3. Professional Profile (High Fidelity)

```
┌─────────────────────────────────────────┐
│ ←                          ⋮  ❤️        │
├─────────────────────────────────────────┤
│                                         │
│     ┌───────────────────┐               │
│     │                   │               │
│     │   [Foto Perfil]   │               │
│     │                   │               │
│     └───────────────────┘               │
│                                         │
│        José Ramírez  ✅                 │
│        Carpintero                       │
│        ⭐ 4.9 (127 reviews)             │
│        📍 2.3 km • Urdesa               │
│        💼 20 años experiencia           │
│                                         │
│ ┌─────┬─────────┬─────────┐            │
│ │ 💬  │   📞    │ Cotizar │            │
│ │Chat │ Llamar  │         │            │
│ └─────┴─────────┴─────────┘            │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ [Portfolio] Servicios Reviews Cursos    │ ← Tabs
│ ▔▔▔▔▔▔▔▔                               │
│                                         │
│ Trabajos realizados:                    │
│                                         │
│ ┌────────┬────────┬────────┐           │
│ │        │        │        │           │
│ │ [IMG]  │ [IMG]  │ [IMG]  │           │
│ │        │        │        │           │
│ │        │        │        │           │
│ ├────────┼────────┼────────┤           │
│ │        │        │        │           │
│ │ [IMG]  │ [IMG]  │ [IMG]  │           │
│ │        │        │        │           │
│ │        │        │        │           │
│ ├────────┼────────┼────────┤           │
│ │        │        │        │           │
│ │ [IMG]  │ [IMG]  │ [IMG]  │           │
│ │        │        │        │           │
│ └────────┴────────┴────────┘           │
│                                         │
│ [Ver todos →]                           │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Sobre mí:                               │
│                                         │
│ Carpintero con 20 años de experiencia   │
│ especializado en muebles a medida,      │
│ cocinas integrales y restauración.      │
│ Trabajo con maderas nobles y ofrezco    │
│ garantía en todos mis trabajos.         │
│                                         │
│ Especialidades:                         │
│ • Muebles a medida                      │
│ • Cocinas integrales                    │
│ • Closets y vestidores                  │
│ • Restauración de muebles               │
│                                         │
│ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  │
│                                         │
│ Cursos que ofrece (2):                  │
│                                         │
│ ┌─────────────────────────────────────┐ │
│ │ [IMG] Carpintería Básica            │ │
│ │       4 sesiones • $80              │ │
│ │       ⭐ 4.9 (24 estudiantes)       │ │
│ │       [Ver curso →]                 │ │
│ └─────────────────────────────────────┘ │
│                                         │
│ [Ver todos los cursos →]                │
│                                         │
├─────────────────────────────────────────┤
│  [🏠]     [🔍]     [💼]     [💬]  [👤] │
└─────────────────────────────────────────┘
```

---

## Prototipo Interactivo

### 🎬 Flujos a Prototipar

#### FLUJO 1: Onboarding → Home (2 min)

```
Screens:
1. Splash/Welcome
2. Onboarding 1 (Ilustración + texto)
3. Onboarding 2 (Seleccionar rol)
4. Onboarding 3 (Ubicación)
5. Registro
6. Home

Interactions:
- Splash → Auto transition (2s) → Onboarding 1
- Onboarding 1-3: Swipe horizontal O botón "Continuar"
  • Animation: Move In from Right
  • Duration: 400ms
  • Easing: Ease out
- Skip button: Jump directo a Registro
- Registro → Home: Fade transition (500ms)

Micro-interactions:
- Progress dots animate
- Buttons hover effect (scale 1.05)
- Form inputs focus state
```

#### FLUJO 2: Buscar y Ver Profesional (3 min)

```
Screens:
1. Home
2. Search Results
3. Professional Profile
4. Portfolio Gallery (overlay)
5. Request Quote

Interactions:

Home → Search:
- Click en categoría → Navigate to Search Results
  • Passing data: Category name
  • Animation: Move In from Right, 300ms

Search Results:
- Professional Card: On Click → Profile
  • Animation: Move In from Right, 300ms
- Heart icon: On Click → Fill animation
  • Smart Animate, 200ms

Professional Profile:
- Tabs: On Click → Change content
  • Smart Animate between tabs, 300ms
- Portfolio photo: On Click → Open Overlay Gallery
  • Animation: Scale up + Dissolve, 400ms
  • Background: Black 80% opacity
  • Swipe to navigate photos
  • Close button o tap outside
- "Cotizar" button: On Click → Request Quote
  • Animation: Move In from Bottom, 400ms

Request Quote:
- Form interactions:
  • Input focus states
  • Photo upload: Click → Show picker (overlay)
  • Date picker: Slide up overlay
- Submit button: On Click → Loading → Success
  • Loading: Spinner 2s
  • Success: Checkmark animation → Navigate Home
```

#### FLUJO 3: Ver y Comprar Curso (2.5 min)

```
Screens:
1. Home (Tab Cursos)
2. Course List
3. Course Detail
4. Enrollment Form
5. Payment
6. Confirmation

Interactions:

Home → Courses:
- Tab switch: Smart Animate, 200ms
- Course card: On Click → Course Detail
  • Move In from Right, 300ms

Course Detail:
- Hero image: Parallax scroll effect
- Tabs (Descripción/Temario/Reviews): Smart Animate
- "Inscribirme" button: Sticky bottom
  • On Click → Enrollment Form (Slide up overlay)

Enrollment Form:
- Date selector: Horizontal scroll
- Confirm: On Click → Payment
  • Slide up, 400ms

Payment:
- Payment method cards: On Click → Select (checkmark)
- "Pagar" button: On Click → Processing → Success
  • Processing: 2s loading
  • Success: Confetti animation + Navigate Confirmation

Confirmation:
- Success animation:
  • Checkmark: Scale 0 → 1, Spring, 600ms
  • Confetti particles fade in/out
- "Add to calendar" button
- "Volver a inicio" → Navigate Home
```

#### FLUJO 4: Chat con Profesional (1.5 min)

```
Screens:
1. Professional Profile
2. Chat List (si viene de nav)
3. Chat Conversation

Interactions:

Profile → Chat:
- Chat button: On Click → Chat Conversation
  • Move In from Right, 300ms
  • If first time: Create new conversation

Chat Conversation:
- Message input:
  • On focus: Keyboard pushes content up
  • Character count: Updates live
- Send button:
  • On Click: Message bubble appears
    • Slide in from right, 200ms
    • Delivered checkmark appears (fade in)
- Photo attachment:
  • On Click: Photo picker overlay
  • Selected photo: Preview thumbnail
- Back: Navigate to Chat List or Profile
```

---

## Micro-interactions

### 1. Card Hover/Press Effects

```
Professional Card:
- Idle: Shadow 0 2px 12px rgba(0,0,0,0.08)
- Hover: 
  • Shadow 0 
│