# Padel Scoreboard

Marcador digital para partidos de pádel y retas. Funciona como PWA (Progressive Web App), se puede instalar en el celular y usar sin conexión.

**Demo en vivo:** [https://prime-leads-app.github.io/padel-app/](https://prime-leads-app.github.io/padel-app/)

## Modos de juego

### Padel (Normal)

Formato oficial de pádel con sets, juegos y puntos.

- **Puntos:** 0 → 15 → 30 → 40 → gana juego
- **Juegos por set:** 6 o 4 (configurable)
- **Sets para ganar:** 1, 2 o 3 (configurable)
- **Empate a 40:** Punto de Oro o Ventaja
- **Tie-break:** Se activa automáticamente si empatan en juegos (6-6 o 4-4)

### Padel (Retas)

Formato informal popular en México. Se juega un número fijo de juegos sin sets.

- **Juegos fijos:** 4, 6 u 8 (configurable)
- **Puntos:** Igual que pádel oficial (0 → 15 → 30 → 40)
- **Desempate:** Si empatan (ej: 3-3 en reta de 6), se juega un juego extra
- **Fin del partido:**
  - **Todos:** Se juegan todos los juegos, gana quien tenga más al final
  - **Anticipado:** Termina cuando un equipo tiene mayoría matemática

### Libre

Modo libre para cualquier actividad. Cada toque suma 1 punto. El primero en llegar a 30 puntos gana.

## Funcionalidades

- **Nombres editables:** Modo Jugadores (2 nombres por equipo) o Equipos (1 nombre por equipo)
- **Sonidos diferenciados:** Cada equipo tiene un tono distinto al anotar
- **Indicador de saque:** Muestra qué equipo tiene el saque
- **Historial:** Registro de todos los puntos con hora, separado por modo
- **Deshacer:** Permite revertir el último punto anotado
- **Reiniciar:** Resetea solo los marcadores, mantiene nombres
- **Limpiar:** Resetea marcadores y nombres
- **Persistencia:** Todo se guarda en localStorage, no se pierde al cerrar
- **PWA:** Se puede instalar como app en el celular
- **Cooldown de 3 segundos:** Evita toques accidentales

## Navegación

Toda la app se controla desde el menú hamburguesa (icono ☰) en la parte superior:

- **Configuración** - Muestra/oculta todas las opciones de juego (modo, nombres, formato, etc.)
- **Ayuda opciones** - Explica qué significa cada opción de configuración
- **Cómo jugar pádel/retas/libre** - Reglas y ejemplos de cada modo
- **Historial** - Registro de puntos anotados

## Configuración

Accesible desde el menú hamburguesa > Configuración:

| Opción | Valores | Descripción |
|--------|---------|-------------|
| Modo | Padel / Libre | Tipo de marcador |
| Nombres | Jugadores / Equipos | 2 nombres por equipo o 1 nombre de equipo |
| Formato | Normal / Retas | Formato de partido (solo Padel) |
| Sets | 1, 2, 3 | Sets para ganar (solo Normal) |
| Juegos | 6, 4 | Juegos por set (solo Normal) |
| Juegos | 4, 6, 8 | Juegos fijos (solo Retas) |
| Fin | Todos / Anticipado | Jugar todos los juegos o terminar con mayoría (solo Retas) |
| 40-40 | Oro / Ventaja | Qué pasa en empate a 40 |

## Tecnología

- HTML, CSS, JavaScript (vanilla, sin frameworks)
- Bootstrap 5 (solo CSS)
- Web Audio API para sonidos
- Service Worker para uso offline
- LocalStorage para persistencia

## Contribuir

1. Fork del repositorio
2. Crea tu rama (`git checkout -b feature/nueva-funcionalidad`)
3. Commit de tus cambios (`git commit -m 'Agregar nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

Para sugerencias directas: [Enviar mensaje por WhatsApp](https://wa.me/525951109110?text=Hola,%20quiero%20aportar%20una%20sugerencia%20para%20la%20app%20padel%20scoreboard)

## Autor

Desarrollado por **FrankZamora**
