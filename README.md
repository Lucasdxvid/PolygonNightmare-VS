# 🎮 PolygonNightmare

**PolygonNightmare** es un videojuego indie en desarrollo, de género **terror cooperativo**, con estética **low-poly estilo PS1**.  
El proyecto está orientado tanto al **aprendizaje en Unity** como a la creación de una experiencia jugable original que, a futuro, podría publicarse en Steam.

---

## 🧩 Concepto del juego

Los jugadores encarnan **formas geométricas básicas** en un mundo poligonal lleno de acertijos y un monstruo que los persigue.  
Cada clase tiene habilidades únicas basadas en su geometría:

- 🟥 **Cubo** → fuerte y estable, puede activar placas de presión y empujar bloques.  
- 🔺 **Triángulo** → encaja en ranuras, trepa pendientes y activa mecanismos puntiagudos.  
- 🟢 **Esfera** → se mueve rodando, entra en túneles circulares y gana velocidad.  

El enemigo principal es un **polígono glitch-inestable**, que cambia de forma y rompe las reglas del espacio, generando tensión y atmósfera de horror.

---

## ✨ Características clave (planeadas)

- Cooperativo (2–3 jugadores) con mecánicas complementarias.  
- Estética retro PS1: low poly, texturas pixeladas, jitter de cámara.  
- Puzzles que requieren cooperación entre formas geométricas.  
- Monstruo con comportamiento impredecible y visuales "glitcheados".  
- Ambientación minimalista y atmosférica.  

---

## 📂 Organización del proyecto

El repositorio contiene principalmente **código C# y documentación**.  
Los **assets y escenas** son gestionados por Unity/Plastic SCM.  

Estructura básica (resumida):  
```
Assets/Scripts/        # Código C# del juego
Assets/Scenes/         # Escenas (Unity controla)
Assets/Prefabs/        # Prefabs de jugadores, enemigos, entorno
Assets/Materials/      # Materiales estilo PS1
Assets/Audio/          # Sonidos y música
```

Para detalles técnicos, ver:  
- [`FOLDER_STRUCTURE.md`](./Assets/FOLDER_STRUCTURE.md)  
- [`COPILOT_SAFETY_GUIDE.md`](./COPILOT_SAFETY_GUIDE.md)  

---

## 🛠️ Tecnologías y herramientas

- **Unity (URP, LTS)** → motor principal.  
- **C#** → scripts y lógica de juego.  
- **VS Code + Copilot** → edición de código.  
- **Git/GitHub** → control de versiones de código.  
- **Plastic SCM** → control de versiones de assets de Unity.  

---

## 🚀 Estado del proyecto

- [x] Configuración inicial de Unity y VS Code.  
- [x] Control de versiones híbrido Git + Plastic.  
- [x] Documentación de estructura y guías de seguridad.  
- [x] Extensiones y linting configurado.
- [ ] Scripts base de jugadores (Cubo, Triángulo, Esfera).
- [ ] Sistema de movimiento básico.  
- [ ] Cámara estilo PS1.  
- [ ] Prototipo de enemigo glitch.  
- [ ] Mecánicas cooperativas básicas.
- [ ] Integración multijugador.  
- [ ] Primer nivel jugable.  
- [ ] Shaders estilo PS1.
- [ ] Sistema de audio atmosférico.

---

## 🎯 Mecánicas únicas del juego

### Sistema de Formas Cooperativas
Cada jugador tiene acceso a áreas y mecánicas específicas según su geometría:

- **Espacios cuadrados** → Solo accesibles para Cubos
- **Ranuras triangulares** → Solo accesibles para Triángulos  
- **Túneles circulares** → Solo accesibles para Esferas
- **Puzzles cooperativos** → Requieren múltiples formas trabajando juntas

### Enemigo Glitch
- Cambia de forma impredeciblemente
- Rompe las reglas del espacio poligonal
- Crea distorsiones visuales y auditivas
- Persigue a los jugadores de manera inteligente

---

## 🔧 Configuración de desarrollo

### Prerrequisitos
- Unity 2022.3 LTS o superior
- Visual Studio Code
- Git instalado
- Extensiones recomendadas: C#, Unity Snippets, GitLens

### Setup del proyecto
1. Clonar este repositorio
2. Abrir la carpeta en Unity
3. Configurar Plastic SCM para assets
4. Instalar extensiones de VS Code recomendadas

---

## 📋 Convenciones del proyecto

### Código
- **Namespace**: `PolygonNightmare.{Modulo}`
- **Clases**: PascalCase (`PlayerController`)
- **Variables**: camelCase (`playerSpeed`)
- **Constantes**: UPPER_CASE (`MAX_PLAYERS`)

### Assets
- **Prefabs**: `NombreDescriptivo_Prefab.prefab`
- **Materials**: `NombreDescriptivo_Material.mat`
- **Scripts**: `NombreClase.cs`

---

## 🤝 Contribuciones

Este es un proyecto de aprendizaje personal, pero si estás interesado en contribuir:

1. Revisa [`COPILOT_SAFETY_GUIDE.md`](./COPILOT_SAFETY_GUIDE.md) para entender qué archivos son modificables
2. Solo trabaja con scripts C# en `Assets/Scripts/`
3. Sigue las convenciones de nomenclatura establecidas
4. Documenta tu código con comentarios XML

---

## 📜 Licencia

Actualmente el proyecto es **experimental y de aprendizaje**, sin licencia pública definida.  
El contenido puede cambiar a medida que avance el desarrollo.

---

## 👤 Autor

Proyecto creado por **Lucasdxvid**, con ayuda de **ChatGPT + GitHub Copilot** para prototipado de código y documentación.

---

## 🎮 Inspiración

- **Estética**: Silent Hill PS1, LSD Dream Emulator, Antichamber
- **Mecánicas**: Portal series, It Takes Two, A Way Out
- **Horror**: Liminal spaces, geometric horror, glitch aesthetics

---

*"En un mundo donde la geometría define las reglas, ¿qué sucede cuando algo las rompe?"*
