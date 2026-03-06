# Plan de Mejoras - Padel Scoreboard

## Fase 1: Correcciones (bugs actuales)

- [x] 1.1 Winner score en retas muestra "Sets: 0-0" en vez de "Juegos: X-X"
- [x] 1.2 "Ayuda opciones" dice "con 2 de ventaja" en Juegos 6 y 4 (ya se corrigio en reglas pero no en ayuda)
- [x] 1.3 "Ayuda opciones" no menciona Formato (Normal/Retas), Puntos de Libre, ni Fin (Todos/Anticipado)

## Fase 2: Feedback visual y haptico

- [x] 2.1 Cooldown con indicador visual (barra de progreso o timer que muestre los 3 segundos)
- [x] 2.2 Vibracion al anotar punto (navigator.vibrate)

## Fase 3: Funcionalidad de partido

- [x] 3.1 Temporizador de partido (inicia al primer punto, se detiene al terminar)
- [x] 3.2 Compartir resultado final (Web Share API / copiar al clipboard)

## Fase 4: Historial de partidos

- [ ] 4.1 Guardar partidos terminados con fecha, resultado, nombres y modo
- [ ] 4.2 Vista de historial de partidos (lista de partidos anteriores)

## Fase 5: Mejoras visuales

- [ ] 5.1 Modo landscape en mobile (tarjetas lado a lado)
- [ ] 5.2 Modo claro/oscuro (toggle de tema para uso al aire libre)

---

Orden de implementacion: Fase 1 > 2 > 3 > 4 > 5
Cada fase se completa y se hace commit antes de pasar a la siguiente.
