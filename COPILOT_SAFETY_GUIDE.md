# 🚨 COPILOT SAFETY GUIDE - PolygonNightmare

**IMPORTANTE: Este documento define qué archivos pueden y NO pueden ser modificados por GitHub Copilot y herramientas de IA.**

## ❌ NUNCA MODIFICAR - Control de Unity/Plastic SCM

### 📁 Carpetas PROHIBIDAS para Copilot:
```
Assets/ (excepto Scripts/ y FOLDER_STRUCTURE.md)
├── Audio/              ❌ Unity maneja
├── Data/               ❌ Unity maneja  
├── Materials/          ❌ Unity maneja
├── Plugins/            ❌ Unity maneja
├── PostProcessing/     ❌ Unity maneja
├── Prefabs/            ❌ Unity maneja
├── Scenes/             ❌ Unity maneja
├── Settings/           ❌ Unity maneja
├── Shaders/            ❌ Unity maneja
├── Textures/           ❌ Unity maneja
└── TutorialInfo/       ❌ Unity maneja

ProjectSettings/        ❌ Unity maneja completamente
Packages/              ❌ Unity maneja completamente
Library/               ❌ Unity genera automáticamente
Temp/                  ❌ Unity genera automáticamente
Logs/                  ❌ Unity genera automáticamente
UserSettings/          ❌ Unity genera automáticamente
```

### 📄 Archivos PROHIBIDOS para Copilot:
```
*.meta                 ❌ Metadatos de Unity
*.asset                ❌ Assets de Unity
*.unity                ❌ Escenas de Unity
*.prefab               ❌ Prefabs de Unity
*.mat                  ❌ Materiales de Unity
*.controller           ❌ Animadores de Unity
*.anim                 ❌ Animaciones de Unity
*.mixer                ❌ Audio mixers de Unity
*.playable             ❌ Timeline assets de Unity
*.signal               ❌ Signals de Unity
*.preset               ❌ Presets de Unity
*.lighting             ❌ Lighting settings de Unity
*.giparams             ❌ Global illumination params
ignore.conf            ❌ Configuración de Plastic SCM
```

### 🎯 Archivos de Configuración Unity:
```
manifest.json          ❌ Package Manager de Unity
packages-lock.json     ❌ Package Manager de Unity
ProjectVersion.txt     ❌ Versión del proyecto Unity
```

## ✅ PERMITIDO MODIFICAR - Control de Git/VS Code

### 📁 Carpetas PERMITIDAS para Copilot:
```
Assets/Scripts/        ✅ Código C# del juego
├── Player/            ✅ Scripts de jugadores
├── Enemies/           ✅ Scripts de enemigos
├── GameManagement/    ✅ Scripts de managers
├── UI/                ✅ Scripts de interfaz
└── Utils/             ✅ Scripts de utilidades

.vscode/               ✅ Configuración VS Code
```

### 📄 Archivos PERMITIDOS para Copilot:
```
Assets/Scripts/**/*.cs     ✅ Scripts de C#
Assets/FOLDER_STRUCTURE.md ✅ Documentación
.gitignore                 ✅ Control de versiones
.editorconfig             ✅ Configuración de formato
PolygonNightmare.ruleset  ✅ Reglas de análisis
COPILOT_SAFETY_GUIDE.md   ✅ Esta guía
README.md                 ✅ Documentación del proyecto
.vscode/settings.json     ✅ Configuración VS Code
.vscode/launch.json       ✅ Configuración debug
.vscode/tasks.json        ✅ Tareas de VS Code
```

## 🔒 REGLAS ESTRICTAS PARA COPILOT

### 1. 🚫 NUNCA crear, modificar o eliminar:
- Archivos `.meta`
- Archivos `.asset`
- Archivos `.unity` (escenas)
- Archivos `.prefab`
- Archivos `.mat` (materiales)
- Cualquier archivo en `ProjectSettings/`
- Cualquier archivo en `Packages/`
- Configuraciones de Plastic SCM

### 2. ✅ SOLO trabajar con:
- Scripts C# en `Assets/Scripts/`
- Archivos de configuración del proyecto (`.gitignore`, `.editorconfig`, etc.)
- Documentación en Markdown
- Configuraciones de VS Code

### 3. 🔍 ANTES de modificar cualquier archivo:
- Verificar que esté en la lista PERMITIDA
- Confirmar que no tiene extensión `.meta`
- Asegurarse que no está en carpetas controladas por Unity

### 4. 📝 Al crear nuevos archivos:
- SOLO crear archivos `.cs` en `Assets/Scripts/`
- SOLO crear documentación `.md` en la raíz del proyecto
- NUNCA crear archivos Unity (prefabs, materials, etc.)

## ⚠️ SEÑALES DE ALERTA

### 🚨 SI VES ESTO, DETENTE:
- Copilot sugiere modificar un archivo `.meta`
- Copilot quiere crear un archivo `.prefab`
- Copilot intenta modificar `ProjectSettings/`
- Copilot sugiere cambios en `Packages/`
- Copilot quiere modificar archivos `.asset`
- Copilot sugiere cambios en configuraciones de Unity

### ✋ RESPUESTA RECOMENDADA:
```
"No puedo modificar ese archivo porque está controlado por Unity/Plastic SCM. 
Solo puedo trabajar con scripts C# en Assets/Scripts/ y archivos de configuración del proyecto."
```

## 🎯 FLUJO DE TRABAJO SEGURO

### 1. Para CÓDIGO:
```
✅ Modificar: Assets/Scripts/**/*.cs
✅ Crear: Nuevos scripts en Assets/Scripts/
✅ Documentar: En comentarios XML del código
```

### 2. Para CONFIGURACIÓN:
```
✅ Modificar: .vscode/settings.json
✅ Modificar: .editorconfig
✅ Modificar: PolygonNightmare.ruleset
✅ Modificar: .gitignore
```

### 3. Para DOCUMENTACIÓN:
```
✅ Modificar: *.md en raíz del proyecto
✅ Modificar: Assets/FOLDER_STRUCTURE.md
✅ Crear: Nueva documentación .md
```

## 📋 CHECKLIST ANTES DE CUALQUIER MODIFICACIÓN

- [ ] ¿El archivo está en `Assets/Scripts/`?
- [ ] ¿Es un archivo `.cs`?
- [ ] ¿NO tiene extensión `.meta`?
- [ ] ¿NO está en carpetas controladas por Unity?
- [ ] ¿Es documentación o configuración del proyecto?

**Si alguna respuesta es NO, entonces NO MODIFICAR.**

## 🔧 COMANDOS SEGUROS PARA COPILOT

### ✅ Comandos PERMITIDOS:
```bash
# Crear nuevos scripts
"Crear script PlayerController.cs en Assets/Scripts/Player/"
"Generar clase EnemyAI.cs en Assets/Scripts/Enemies/"

# Modificar configuración
"Actualizar .vscode/settings.json"
"Modificar .gitignore"

# Documentación
"Actualizar FOLDER_STRUCTURE.md"
"Crear README.md"
```

### ❌ Comandos PROHIBIDOS:
```bash
# NO usar estos comandos
"Crear prefab de jugador"
"Modificar material del enemigo"
"Actualizar configuración de Unity"
"Cambiar settings del proyecto"
"Modificar scene principal"
```

## 🎮 RECORDATORIO ESPECÍFICO DEL PROYECTO

Este es un proyecto de **terror cooperativo** donde:
- **Unity/Plastic SCM** maneja assets, prefabs, escenas, materiales
- **Git/GitHub** maneja código C#, configuraciones, documentación
- **Copilot** SOLO debe trabajar con código y configuraciones de desarrollo

### 🏗️ Arquitectura del Juego:
- **Jugadores**: Cubo, Triángulo, Esfera (solo scripts)
- **Mecánicas**: Dependientes de la forma (solo lógica C#)
- **Assets visuales**: Controlados por Unity (NO tocar)

---

**🚨 RECUERDA: Cuando tengas dudas, es mejor NO modificar que arruinar el proyecto.**
