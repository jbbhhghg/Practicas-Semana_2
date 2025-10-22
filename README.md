# Navegación - Prácticas (Stack, Tabs, Drawer)

Este apartado consolida las 3 prácticas: Stack Navigator (Blog App), Tab Navigator (Dashboard App) y Drawer Navigator (Settings App). Cada práctica incluye estructura de archivos, código de ejemplo y checklist de verificación.

Requisitos
- Node.js (16+ recomendado)
- pnpm, npm o yarn
- Expo CLI (no es estrictamente necesario, se usa `npx expo`)

Estructura sugerida

nav-practices/
├── stack-practice/
├── tab-practice/
├── drawer-practice/
└── README.md

Cómo usar (PowerShell en Windows)

# 1. Crear carpeta de proyecto y moverse a ella
mkdir nav-practices; cd nav-practices

# 2. Scaffold con Expo (managed) - con pnpm
npx create-expo-app stack-practice --template expo-template-blank-typescript
# o usar npm: npx create-expo-app stack-practice --template expo-template-blank-typescript

# 3. Repetir para tab-practice y drawer-practice
npx create-expo-app tab-practice --template expo-template-blank-typescript
npx create-expo-app drawer-practice --template expo-template-blank-typescript

Dependencias recomendadas (ejecutar dentro de cada proyecto)
# React Navigation core
pnpm add @react-navigation/native
pnpm add react-native-screens react-native-safe-area-context

# Native stack and bottom tabs / drawer
pnpm add @react-navigation/native-stack @react-navigation/bottom-tabs @react-navigation/drawer

# Gesture and reanimated (necesario para drawer/gestos)
pnpm add react-native-gesture-handler react-native-reanimated

# Icons
pnpm add @expo/vector-icons

Notas importantes
- Añade `react-native-reanimated/plugin` al final de `babel.config.js` si usas Reanimated.
- Reinicia el servidor con `pnpm start --clear` si hay problemas.

Siguiente paso (opcional automático)
Si quieres, puedo generar el scaffold de código TypeScript para las 3 prácticas dentro de `nav-practices` (archivos `App.tsx`, `src/navigation`, `src/screens`, `src/data` con ejemplos). Dime si quieres que lo haga ahora.
