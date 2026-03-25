# Solution: objects-ts

This repository contains the solution for the `objects-ts` project, consolidated into a single Markdown file for easy reading.

## Source Code

### [index.ts](file:///home/andres-david/Descargas/oneClass-ts/src/index.ts)
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

//plantilla

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

//vida('logica de negocio')


//ustedes me van a crear otros dos objetos y los van a recorrer, quiero que los recorran todos..

const jugadores: Jugador[] = [jugador1, jugador2, jugador3];

for (const j of jugadores) {

}
```

## Configuration

### [package.json](file:///home/andres-david/Descargas/oneClass-ts/package.json)
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

### [tsconfig.json](file:///home/andres-david/Descargas/oneClass-ts/tsconfig.json)
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
