# Estructura de Carpetas del Proyecto PolygonNightmare

Este documento describe la organización de carpetas del proyecto para mantener un código limpio y organizado.

## 📁 Assets/Scripts/
Contiene todos los scripts de C# organizados por funcionalidad:

### 🎮 Player/
Scripts relacionados con los jugadores y sus diferentes formas:
- `PlayerController.cs` - Controlador base para todos los jugadores
- `CubePlayer.cs` - Lógica específica para jugadores cubo
- `TrianglePlayer.cs` - Lógica específica para jugadores triángulo  
- `SpherePlayer.cs` - Lógica específica para jugadores esfera
- `PlayerMovement.cs` - Sistema de movimiento
- `PlayerInteraction.cs` - Sistema de interacciones

### 👹 Enemies/
Scripts para enemigos y monstruos:
- `EnemyController.cs` - Controlador base de enemigos
- `EnemyAI.cs` - Inteligencia artificial
- `EnemySpawner.cs` - Sistema de generación de enemigos

### 🎯 GameManagement/
Scripts para la gestión general del juego:
- `GameManager.cs` - Administrador principal del juego
- `LevelManager.cs` - Gestión de niveles
- `ObjectiveManager.cs` - Sistema de objetivos
- `NetworkManager.cs` - Gestión de conexiones multijugador

### 🎨 UI/
Scripts para la interfaz de usuario:
- `MainMenu.cs` - Menú principal
- `HUD.cs` - Interfaz durante el juego
- `InventoryUI.cs` - Interfaz de inventario

### 🔧 Utils/
Scripts de utilidades y herramientas:
- `Extensions.cs` - Métodos de extensión
- `Constants.cs` - Constantes del juego
- `Enums.cs` - Enumeraciones

## 📁 Assets/Scenes/
Escenas organizadas por propósito:

### Menu/
- `MainMenu.unity` - Menú principal del juego
- `OptionsMenu.unity` - Menú de configuraciones
- `CreditsScene.unity` - Pantalla de créditos

### Levels/
- `Level01_Tutorial.unity` - Nivel tutorial
- `Level02_CoopIntro.unity` - Introducción cooperativa
- `Level03_FirstHorror.unity` - Primer nivel de terror

### Multiplayer/
- `MultiplayerLobby.unity` - Sala de espera multijugador
- `NetworkTestScene.unity` - Escena de pruebas de red

### Testing/
- `PlayerTestScene.unity` - Pruebas de mecánicas de jugador
- `EnemyTestScene.unity` - Pruebas de IA de enemigos
- `PhysicsTestScene.unity` - Pruebas de físicas

## 📁 Assets/Data/
ScriptableObjects para configuraciones:

### PlayerStats/
- `CubePlayerStats.asset` - Estadísticas del jugador cubo
- `TrianglePlayerStats.asset` - Estadísticas del jugador triángulo
- `SpherePlayerStats.asset` - Estadísticas del jugador esfera

### EnemyStats/
- `BasicEnemyStats.asset` - Configuración de enemigo básico
- `BossEnemyStats.asset` - Configuración de jefes

### LevelConfig/
- `Level01Config.asset` - Configuración del nivel 1
- `DifficultySettings.asset` - Configuraciones de dificultad

### GameSettings/
- `AudioSettings.asset` - Configuraciones de audio
- `GraphicsSettings.asset` - Configuraciones gráficas

## 📁 Assets/Prefabs/
Prefabs organizados por categoría:

### Players/
- `CubePlayer_Prefab.prefab` - Prefab del jugador cubo
- `TrianglePlayer_Prefab.prefab` - Prefab del jugador triángulo
- `SpherePlayer_Prefab.prefab` - Prefab del jugador esfera

### Enemies/
- `BasicEnemy_Prefab.prefab` - Enemigo básico
- `HorrorMonster_Prefab.prefab` - Monstruo principal

### Environment/
- `PolygonWall_Prefab.prefab` - Muros poligonales
- `InteractableObject_Prefab.prefab` - Objetos interactuables
- `LevelGeometry_Prefab.prefab` - Geometría de niveles

## 📁 Assets/Materials/
Materiales para el estilo PS1 y efectos visuales:
- `PlayerCubeMaterial.mat` - Material del jugador cubo
- `WallMaterial_PS1.mat` - Material de paredes estilo PS1
- `EnemyMaterial_Horror.mat` - Material de enemigos

## 📁 Assets/Textures/
Texturas organizadas por uso:
- `player_cube_texture.png` - Textura del jugador cubo
- `wall_texture_01.png` - Textura de pared básica
- `horror_enemy_texture.png` - Textura del enemigo principal

## 📁 Assets/Shaders/
Shaders personalizados para el estilo visual:

### PS1Style/
- `PS1_Unlit.shader` - Shader sin iluminación estilo PS1
- `PS1_VertexLit.shader` - Shader con vertex lighting PS1
- `PixelationEffect.shader` - Efecto de pixelación

## 📁 Assets/PostProcessing/
Efectos de post-procesamiento:

### Profiles/
- `PS1_HorrorProfile.asset` - Perfil de post-procesamiento estilo PS1
- `MenuProfile.asset` - Perfil para menús

### CustomEffects/
- Scripts de efectos personalizados de post-procesamiento

## 📁 Assets/Audio/
### SFX/
- `player_footstep.wav` - Pasos del jugador
- `enemy_growl.wav` - Gruñido del enemigo
- `interaction_sound.wav` - Sonido de interacción

### Music/
- `main_menu_theme.ogg` - Música del menú principal
- `horror_ambient.ogg` - Ambiente de terror
- `victory_theme.ogg` - Música de victoria

## 📁 Assets/Plugins/
### ThirdParty/
- Plugins y assets de terceros (Photon, ProBuilder, etc.)

## 🎯 Convenciones de Nomenclatura

### Scripts (C#):
- **PascalCase** para clases: `PlayerController`, `EnemyAI`
- **camelCase** para variables y métodos: `playerSpeed`, `GetCurrentHealth()`
- **UPPER_CASE** para constantes: `MAX_PLAYERS`, `DEFAULT_SPEED`

### Assets:
- **PascalCase** para prefabs: `CubePlayer_Prefab`, `TriangleEnemy_Prefab`
- **lowercase_snake_case** para texturas: `wall_texture_01`, `player_cube_material`
- **PascalCase** para materiales: `WallMaterial`, `PlayerCubeMaterial`
- **PascalCase** para ScriptableObjects: `CubePlayerStats`, `Level01Config`

### Scenes:
- **PascalCase**: `MainMenu`, `Level01_Tutorial`, `MultiplayerLobby`

### Archivos de Audio:
- **lowercase_snake_case**: `player_footstep`, `horror_ambient`, `enemy_growl`

## 🔧 Mejores Prácticas

1. **Un script por archivo** - Cada clase en su propio archivo
2. **Namespace consistente** - Usar `PolygonNightmare.Player`, `PolygonNightmare.Enemies`, etc.
3. **Comentarios XML** - Documentar métodos públicos
4. **Separación de responsabilidades** - Cada script tiene una función específica
5. **Prefabs reutilizables** - Crear prefabs para elementos comunes
6. **Versionado de assets** - Numerar versiones de texturas/modelos
7. **ScriptableObjects para datos** - Usar para configuraciones en lugar de hardcodear valores
8. **Organización por funcionalidad** - Agrupar archivos relacionados en las mismas carpetas
9. **Naming consistente** - Seguir las convenciones establecidas sin excepción
10. **Documentación actualizada** - Mantener este archivo actualizado con cambios

## 📋 TODO Initial Tasks
- [ ] Crear scripts base para cada tipo de jugador
- [ ] Implementar sistema de movimiento básico
- [ ] Crear prefabs de jugadores básicos
- [ ] Configurar escena de pruebas inicial
- [ ] Crear ScriptableObjects para estadísticas de jugadores
- [ ] Implementar shaders básicos estilo PS1
- [ ] Configurar perfil de post-procesamiento inicial

## 🎮 Estructura Específica del Juego

### Mecánicas por Forma de Jugador:
- **Cubo**: Puede pasar por espacios cuadrados, activar interruptores de presión
- **Triángulo**: Puede pasar por espacios triangulares, activar mecanismos puntiagudos
- **Esfera**: Puede rodar rápidamente, pasar por túneles circulares

### Sistema de Objetivos Cooperativos:
- Objetivos que requieren formas específicas
- Puzzles que necesitan múltiples jugadores
- Áreas accesibles solo para ciertas formas
