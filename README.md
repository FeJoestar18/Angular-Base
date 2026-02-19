# Angular-Base

[![Angular Version](https://img.shields.io/badge/Angular-21.1-red.svg)](https://angular.io/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.9-blue.svg)](https://www.typescriptlang.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js Version](https://img.shields.io/badge/Node.js-24.x-green.svg)](https://nodejs.org/)

## Sobre o Projeto

**Angular-Base** é um template/boilerplate profissional para iniciar projetos Angular rapidamente com as melhores práticas já configuradas. Este projeto oferece uma estrutura sólida e organizada, permitindo que você comece a desenvolver imediatamente sem se preocupar com configurações iniciais.

O projeto inclui configurações otimizadas de TypeScript, linting com ESLint, formatação de código com Prettier, e testes prontos para uso, proporcionando um ambiente de desenvolvimento consistente e produtivo.

## Features

-  **Angular 21.1** - Última versão do framework com recursos modernos
-  **Configuração Completa** - TypeScript, ESLint e Prettier pré-configurados
-  **Strict Mode** - TypeScript em modo strict para maior segurança de tipos
-  **SCSS Support** - Pré-processador CSS configurado
-  **Testing Ready** - Vitest configurado para testes unitários
-  **Routing** - Angular Router configurado e pronto para uso
-  **EditorConfig** - Consistência de código entre diferentes editores
-  **Build Otimizado** - Configurações de build para produção
-  **Code Quality** - Linting e formatação automatizados
-  **Scripts NPM** - Comandos úteis para desenvolvimento

## Tecnologias

Este projeto utiliza as seguintes tecnologias:

- **[Angular](https://angular.io/)** ^21.1.0 - Framework web progressivo
- **[TypeScript](https://www.typescriptlang.org/)** ~5.9.2 - JavaScript tipado
- **[RxJS](https://rxjs.dev/)** ~7.8.0 - Programação reativa
- **[SCSS](https://sass-lang.com/)** - Pré-processador CSS
- **[Vitest](https://vitest.dev/)** ^4.0.8 - Framework de testes
- **[ESLint](https://eslint.org/)** - Linting de código
- **[Prettier](https://prettier.io/)** - Formatação de código

## Pré-requisitos

Antes de começar, certifique-se de ter instalado:

- **Node.js** (versão 24.x ou superior)
- **npm** (versão 11.x ou superior) ou **yarn**
- **Angular CLI** (opcional, mas recomendado)

Para instalar o Angular CLI globalmente:

```bash
npm install -g @angular/cli
```

## Como Usar

### Instalação

Clone o repositório e instale as dependências:

```bash
# Clone o repositório
git clone https://github.com/FeJoestar18/Angular-Base.git

# Entre na pasta do projeto
cd Angular-Base

# Instale as dependências
npm install
```

### Desenvolvimento

Inicie o servidor de desenvolvimento:

```bash
# Inicia o servidor de desenvolvimento
npm start

# Ou com o Angular CLI
ng serve

# Para abrir automaticamente no navegador
npm run dev
```

O aplicativo estará disponível em `http://localhost:4200/`. A aplicação será recarregada automaticamente quando você modificar qualquer arquivo.

### Build

Para compilar o projeto para produção:

```bash
# Build para produção
npm run build:prod

# Ou usando o Angular CLI
ng build --configuration production
```

Os arquivos compilados serão gerados na pasta `dist/`.

### Testes

Execute os testes unitários:

```bash
# Executar testes unitários
npm test

# Executar testes com coverage
npm run test:coverage
```

### Linting e Formatação

Para manter a qualidade do código:

```bash
# Executar linting
npm run lint

# Formatar código
npm run format

# Verificar formatação sem modificar
npm run format:check
```

## Estrutura do Projeto

```
Angular-Base/
├── src/
│   ├── app/
│   │   ├── app.config.ts      # Configuração da aplicação
│   │   ├── app.routes.ts      # Definição de rotas
│   │   ├── app.ts             # Componente principal
│   │   ├── app.html           # Template principal
│   │   ├── app.scss           # Estilos principais
│   │   └── app.spec.ts        # Testes do componente
│   ├── assets/                # Recursos estáticos
│   ├── index.html             # HTML principal
│   ├── main.ts                # Ponto de entrada da aplicação
│   └── styles.scss            # Estilos globais
├── public/
│   └── favicon.ico            # Ícone da aplicação
├── .editorconfig              # Configuração do editor
├── .gitignore                 # Arquivos ignorados pelo Git
├── .prettierrc                # Configuração do Prettier
├── angular.json               # Configuração do Angular
├── eslint.config.js           # Configuração do ESLint
├── package.json               # Dependências e scripts
├── tsconfig.json              # Configuração do TypeScript
├── tsconfig.app.json          # Config TypeScript para app
├── tsconfig.spec.json         # Config TypeScript para testes
└── README.md                  # Este arquivo
```

## Como Contribuir

Contribuições são sempre bem-vindas! Se você deseja contribuir com este projeto:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

Para mais detalhes sobre como contribuir, consulte o arquivo [CONTRIBUTING.md](CONTRIBUTING.md).

## Scripts Disponíveis

| Script | Descrição |
|--------|-----------|
| `npm start` | Inicia o servidor de desenvolvimento |
| `npm run dev` | Inicia o servidor e abre no navegador |
| `npm run build` | Build de desenvolvimento |
| `npm run build:prod` | Build otimizado para produção |
| `npm test` | Executa os testes unitários |
| `npm run test:coverage` | Executa testes com relatório de cobertura |
| `npm run lint` | Executa o linting do código |
| `npm run format` | Formata o código com Prettier |
| `npm run format:check` | Verifica a formatação do código |

## Configurações

### TypeScript

O projeto está configurado com **Strict Mode** habilitado, garantindo maior segurança de tipos e qualidade de código. As configurações incluem:

- `strict: true`
- `noImplicitOverride: true`
- `noImplicitReturns: true`
- `noFallthroughCasesInSwitch: true`

### ESLint

ESLint está configurado com as regras recomendadas para Angular e TypeScript, incluindo:

- Verificação de seletores de componentes e diretivas
- Detecção de código não utilizado
- Boas práticas do Angular

### Prettier

Prettier está configurado para manter um estilo de código consistente:

- Single quotes
- Print width: 100 caracteres
- Trailing commas: ES5
- Parser especial para templates Angular

## Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## Autor

**FeJoestar18** (Felipe Amaro Souza de Jesus)

- GitHub: [@FeJoestar18](https://github.com/FeJoestar18)
- Projeto: [Angular-Base](https://github.com/FeJoestar18/Angular-Base)

## Agradecimentos

- Comunidade Angular pela excelente documentação
- Todos os contribuidores que ajudam a melhorar este projeto

## ⭐ Mostre seu apoio

Se este projeto te ajudou, considere dar uma ⭐️ no repositório!

---

<div align="center">
  Feitopor <a href="https://github.com/FeJoestar18">FeJoestar18</a>
</div>
