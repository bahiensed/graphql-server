# GraphQL Server  
Just a simple GraphQL server from hero to villain

## Groundwork
### create project folder
```bash
mkdir graphql-server
cd graphql-server
```

### init project
```bash
npm init -y
```

### install some dev dependencies
```bash
npm install --save-dev jest nodemon ts-node-dev typescript
```

### run npm update if deprecated package warning shows
```bash
npm update
```

### install and config eslint
```bash
npm init @eslint/config@latest
```

### install project dependencies
```bash
npm install @apollo/server @graphql-tools/mock @graphql-tools/schema graphql graphql-tag
```

### modify package.json
```bash
{
  "name": "graphql-server",
  "version": "1.0.0",
  "description": "Just a simple GraphQL server from zero to villain",
  "main": "./dist/index.js",
  "scripts": {
    "build": "tsc",
    "dev": "ts-node-dev --respawn ./src/index.ts",
    "start": "node ./dist/index.js",
    "test": "jest"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/bahiensed/graphql-server.git"
  },
  "keywords": [
    "Node",
    "TypeScript",
    "GraphQL",
    "Apollo"
  ],
  "author": "Douglas Bahiense @bahiensed",
  "license": "ISC",
  "bugs": {
    "url": "https://github.com/bahiensed/graphql-server/issues"
  },
  "homepage": "https://github.com/bahiensed/graphql-server#readme",
  "devDependencies": {
    "@eslint/js": "^9.10.0",
    "eslint": "^9.10.0",
    "eslint-plugin-react": "^7.36.1",
    "globals": "^15.9.0",
    "jest": "^29.7.0",
    "ts-node-dev": "^2.0.0",
    "typescript": "^5.6.2",
    "typescript-eslint": "^8.5.0"
  },
  "dependencies": {
    "@apollo/server": "^4.11.0",
    "@graphql-tools/mock": "^9.0.4",
    "@graphql-tools/schema": "^10.0.6",
    "graphql": "^16.9.0",
    "graphql-tag": "^2.12.6"
  }
}
```

### init TypeScript
```bash
npx tsc --init
```

### modify tsconfig.json
```bash
{
  "compilerOptions": {
    "rootDir": "src",
    "outDir": "dist",
    "module": "commonjs",
    "target": "es2020",
    "moduleResolution": "node",
    "esModuleInterop": true,
    "strict": true,
    "skipLibCheck": true,
    "forceConsistentCasingInFileNames": true    
  },
  "include": ["src/**/*.ts"],
  "exclude": ["node_modules"]
}
```

### install GraphQL: Syntax Highlighting in VSCodium
```bash
ext install GraphQL.vscode-graphql-syntax
```

## Hands-on


## run project
### in development:  
```bash
npm run dev
```

### in production:
```bash
npm run build
npm start
```
