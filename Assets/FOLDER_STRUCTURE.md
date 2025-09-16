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

## 📁 Assets/Prefabs/
Prefabs organizados por categoría:

### Players/
Prefabs de los diferentes tipos de jugadores (cubo, triángulo, esfera)

### Enemies/
Prefabs de enemigos y monstruos

### Environment/
Prefabs de elementos del entorno y obstáculos

## 📁 Assets/Materials/
Materiales para el estilo PS1 y efectos visuales

## 📁 Assets/Textures/
Texturas organizadas por uso

## 📁 Assets/Audio/
### SFX/
Efectos de sonido

### Music/
Música de fondo y ambiental

## 🎯 Convenciones de Nomenclatura

### Scripts (C#):
- **PascalCase** para clases: `PlayerController`, `EnemyAI`
- **camelCase** para variables y métodos: `playerSpeed`, `GetCurrentHealth()`
- **UPPER_CASE** para constantes: `MAX_PLAYERS`, `DEFAULT_SPEED`

### Assets:
- **PascalCase** para prefabs: `CubePlayer`, `TriangleEnemy`
- **lowercase_snake_case** para texturas: `wall_texture_01`, `player_cube_material`
- **PascalCase** para materiales: `WallMaterial`, `PlayerCubeMaterial`

### Scenes:
- **PascalCase**: `MainMenu`, `GameLevel01`, `MultiplayerLobby`

## 🔧 Mejores Prácticas

1. **Un script por archivo** - Cada clase en su propio archivo
2. **Namespace consistente** - Usar `PolygonNightmare.Namespace`
3. **Comentarios XML** - Documentar métodos públicos
4. **Separación de responsabilidades** - Cada script tiene una función específica
5. **Prefabs reutilizables** - Crear prefabs para elementos comunes
6. **Versionado de assets** - Numerar versiones de texturas/modelos

## 📋 TODO Initial Tasks
- [ ] Crear scripts base para cada tipo de jugador
- [ ] Implementar sistema de movimiento básico
- [ ] Crear prefabs de jugadores básicos
- [ ] Configurar escena de pruebas inicial
