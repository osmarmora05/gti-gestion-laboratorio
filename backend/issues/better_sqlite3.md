# Error:

```
[INFO] 16:01:38 ts-node-dev ver. 2.0.0 (using ts-node ver. 10.9.2, typescri
Error: Could not locate the bindings file. Tried:
    at bindings (/home/osmar/Documentos/gti-gestion-laboratorio/backend/nod
    at new Database (/home/osmar/Documentos/gti-gestion-laboratorio/backend
    at Object.<anonymous> (/home/osmar/Documentos/gti-gestion-laboratorio/b
    at Module._compile (node:internal/modules/cjs/loader:1705:14)
    at Module._compile (/home/osmar/Documentos/gti-gestion-laboratorio/back
    at Module.m._compile (/tmp/ts-node-dev-hook-27568254291185923.js:69:33)
    at Module._extensions..js (node:internal/modules/cjs/loader:1838:10)
    at require.extensions..jsx.require.extensions..js (/tmp/ts-node-dev-hoo
    at require.extensions.<computed> (/tmp/ts-node-dev-hook-275682542911859
    at Object.nodeDevHook [as .ts] (/home/osmar/Documentos/gti-gestion-labo
[ERROR] 16:01:39 Error: Could not locate the bindings file. Tried:
 → /home/osmar/Documentos/gti-gestion-laboratorio/backend/node_modules/.pnpm/better-sqlite3@11.10.0/node_modules/better-sqlite3/Debug/better_sqlite3.node
 → /home/osmar/Documentos/gti-gestion-laboratorio/backend/node_modules/.pnpm/better-sqlite3@11.10.0/node_modules/better-sqlite3/out/Release/better_sqlite3.node
 → /home/osmar/Documentos/gti-gestion-laboratorio/backend/node_modules/.pnpm/better-sqlite3@11.10.0/node_modules/better-sqlite3/Release/better_sqlite3.node
 → /home/osmar/Documentos/gti-gestion-laboratorio/backend/node_modules/.pnpm/better-sqlite3@11.10.0/node_modules/better-sqlite3/build/default/better_sqlite3.node
 → /home/osmar/Documentos/gti-gestion-laboratorio/backend/node_modules/.pnpm/better-sqlite3@11.10.0/node_modules/better-sqlite3/compiled/22.22.2/linux/x64/better_sqlite3.node
 → /home/osmar/Documentos/gti-gestion-laboratorio/backend/node_modules/.pnpm/better-sqlite3@11.10.0/node_modules/better-sqlite3/addon-build/release/install-root/better_sqlite3.node
 → /home/osmar/Documentos/gti-gestion-laboratorio/backend/node_modules/.pnpm/better-sqlite3@11.10.0/node_modules/better-sqlite3/addon-build/debug/install-root/better_sqlite3.node
 → /home/osmar/Documentos/gti-gestion-laboratorio/backend/node_modules/.pnpm/better-sqlite3@11.10.0/node_modules/better-sqlite3/addon-build/default/install-root/better_sqlite3.node
 → /home/osmar/Documentos/gti-gestion-laboratorio/backend/node_modules/.pnpm/better-sqlite3@11.10.0/node_modules/better-sqlite3/lib/binding/node-v127-linux-x64/better_sqlite3.node
```

Solucion:

1. Seguir la instrucciones [aquí](https://github.com/WiseLibs/better-sqlite3/issues/146#issuecomment-3660887957)

En el caso de encontrarse el siguiente error:

```
sh: línea 1: node-gyp: orden no encontrada
 ELIFECYCLE  Command failed.
```

Tienen que instalar node-gyp. Una forma de hacerlo rapido es instalarlo a nivel de sistema:

```bash
npm install -g node-gyp
```

Aqui queda bajo su rensposabilidad si instalarlo a nivel de sistema o a nivel de proyecto. Ya saben
con lo ultimo hackeos de librerias ...
