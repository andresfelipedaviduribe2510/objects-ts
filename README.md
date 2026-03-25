# Proyecto: objects-ts

> [!IMPORTANT]
> **Instrucciones**: Por favor, completa la implementación de la lógica de negocio y el recorrido de los objetos (jugadores) en este proyecto siguiendo los tipos definidos.

Este repositorio contiene la estructura base y configuración para el proyecto `objects-ts`.

---

## Código Fuente

### `src/index.ts`
```typescript
type Position = {
    linea: string; //"defensa | medio | delantero"
    rol: string; //"defender | filtrar | hacer goles"
}

type Jugador = {
    nombre: string;
    club: string;
    dorsal: number;
    activo: boolean;
    position: Position;
}

// Plantilla inicial

const jugador1: Jugador = {
    nombre: "James rodriguez",
    club: "Seleccion colombia",
    dorsal: 10,
    activo: true,
    position: { linea: "medio campo", rol: "caminar" }
}

const jugador2: Jugador = {
    nombre: "Falcao",
    club: "Seleccion colombia",
    dorsal: 9,
    activo: true,
    position: { linea: "delantero", rol: "hacer goles" }
}

const jugador3: Jugador = {
    nombre: "Ronaldo",
    club: "Real madrid",
    dorsal: 9,
    activo: false,
    position: { linea: "delantero", rol: "ser el mejor del mundo" }
}

// Logica de negocio: Agreguen otros dos objetos y recórranlos todos.

const jugadores: Jugador[] = [jugador1, jugador2, jugador3];

for (const j of jugadores) {
    // Implementar recorrido aquí
}
```

## Configuración del Proyecto

### `package.json`
```json
{
  "name": "oneclass-ts",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "typescript": "^6.0.2"
  }
}
```

### `tsconfig.json`
```json
{
  "compilerOptions": {
    "rootDir": "./src",
    "outDir": "./dist",
    "module": "nodenext",
    "target": "esnext",
    "types": [],
    "sourceMap": true,
    "declaration": true,
    "declarationMap": true,
    "noUncheckedIndexedAccess": true,
    "exactOptionalPropertyTypes": true,
    "strict": true,
    "jsx": "react-jsx",
    "verbatimModuleSyntax": true,
    "isolatedModules": true,
    "noUncheckedSideEffectImports": true,
    "moduleDetection": "force",
    "skipLibCheck": true
  }
}
```
