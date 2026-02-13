# 🤝 Guia de Contribuição

Obrigado por considerar contribuir com o Angular-Base! Este documento fornece diretrizes para contribuir com o projeto.

## 📋 Código de Conduta

Ao participar deste projeto, você concorda em manter um ambiente respeitoso e colaborativo. Seja gentil e profissional em todas as interações.

## 🚀 Como Contribuir

### Reportar Bugs

Se você encontrar um bug, por favor:

1. Verifique se o bug já não foi reportado nas [Issues](https://github.com/FeJoestar18/Angular-Base/issues)
2. Se não existe, crie uma nova issue incluindo:
   - Descrição clara do problema
   - Passos para reproduzir o bug
   - Comportamento esperado vs comportamento atual
   - Versões (Node.js, npm, Angular)
   - Screenshots, se aplicável

### Sugerir Melhorias

Sugestões de melhorias são bem-vindas! Para sugerir uma nova feature:

1. Verifique se a sugestão já não existe nas Issues
2. Crie uma nova issue com a tag `enhancement`
3. Descreva detalhadamente a feature e seus benefícios
4. Explique como ela se encaixa no projeto

### Pull Requests

#### Processo de Desenvolvimento

1. **Fork o repositório**
   ```bash
   # Faça um fork do projeto através do GitHub
   ```

2. **Clone seu fork**
   ```bash
   git clone https://github.com/seu-usuario/Angular-Base.git
   cd Angular-Base
   ```

3. **Crie uma branch para sua feature**
   ```bash
   git checkout -b feature/minha-feature
   # ou
   git checkout -b fix/correcao-bug
   ```

4. **Instale as dependências**
   ```bash
   npm install
   ```

5. **Faça suas alterações**
   - Escreva código limpo e bem documentado
   - Siga as convenções de código do projeto
   - Mantenha as mudanças focadas e atômicas

6. **Teste suas alterações**
   ```bash
   # Execute os testes
   npm test
   
   # Execute o linting
   npm run lint
   
   # Formate o código
   npm run format
   
   # Teste o build
   npm run build:prod
   ```

7. **Commit suas mudanças**
   ```bash
   git add .
   git commit -m "feat: adiciona nova funcionalidade"
   ```

8. **Push para seu fork**
   ```bash
   git push origin feature/minha-feature
   ```

9. **Abra um Pull Request**
   - Vá para o repositório original no GitHub
   - Clique em "New Pull Request"
   - Selecione sua branch
   - Preencha a descrição do PR com detalhes das mudanças

#### Checklist do Pull Request

Antes de enviar seu PR, certifique-se de que:

- [ ] O código segue as convenções do projeto
- [ ] Todos os testes estão passando
- [ ] O linting não apresenta erros
- [ ] O código está formatado corretamente
- [ ] A documentação foi atualizada (se necessário)
- [ ] Os commits seguem o padrão de mensagens
- [ ] A descrição do PR é clara e detalhada

## 📝 Convenções de Código

### TypeScript

- Use TypeScript strict mode
- Sempre defina tipos explícitos quando necessário
- Evite usar `any` - use `unknown` quando o tipo é incerto
- Use arrow functions quando apropriado
- Prefira `const` sobre `let`, evite `var`

### Angular

- Siga as convenções do Angular Style Guide
- Use prefixo `app` para seletores de componentes
- Componentes devem usar kebab-case: `app-meu-componente`
- Classes devem usar PascalCase: `MeuComponente`
- Mantenha componentes simples e focados
- Use serviços para lógica de negócio

### Nomenclatura

- **Variáveis e funções**: camelCase (`minhaVariavel`, `minhaFuncao`)
- **Classes e Interfaces**: PascalCase (`MinhaClasse`, `MinhaInterface`)
- **Constantes**: SCREAMING_SNAKE_CASE (`MINHA_CONSTANTE`)
- **Arquivos**: kebab-case (`meu-componente.ts`)

### Commits

Siga o padrão [Conventional Commits](https://www.conventionalcommits.org/):

```
tipo(escopo): descrição curta

Descrição detalhada (opcional)

Footer (opcional)
```

**Tipos de commit:**

- `feat`: Nova funcionalidade
- `fix`: Correção de bug
- `docs`: Apenas mudanças na documentação
- `style`: Mudanças que não afetam o significado do código (formatação, etc)
- `refactor`: Mudança de código que não corrige bug nem adiciona feature
- `perf`: Mudança que melhora performance
- `test`: Adicionar ou corrigir testes
- `chore`: Mudanças em ferramentas, configurações, etc

**Exemplos:**

```bash
feat(auth): adiciona autenticação com JWT
fix(user): corrige erro ao salvar usuário
docs(readme): atualiza instruções de instalação
style(app): formata código conforme prettier
refactor(service): simplifica lógica de validação
test(user): adiciona testes para serviço de usuário
```

## 🧪 Testes

- Escreva testes para novas funcionalidades
- Mantenha a cobertura de testes alta
- Use nomes descritivos para testes
- Organize testes em blocos lógicos (describe/it)

Exemplo:

```typescript
describe('MeuComponente', () => {
  it('deve criar o componente', () => {
    // teste
  });

  it('deve exibir o título corretamente', () => {
    // teste
  });
});
```

## 📚 Documentação

- Documente funções e métodos complexos com JSDoc
- Atualize o README.md se adicionar novas features
- Mantenha comentários claros e concisos
- Evite comentários óbvios

Exemplo de JSDoc:

```typescript
/**
 * Calcula o total de itens no carrinho
 * @param items - Array de itens do carrinho
 * @returns O valor total calculado
 */
calcularTotal(items: Item[]): number {
  // implementação
}
```

## 🔍 Code Review

Todos os Pull Requests passam por code review. Durante o review:

- Seja receptivo a feedback
- Responda comentários e perguntas
- Faça as alterações solicitadas
- Mantenha a discussão profissional e construtiva

## ⚡ Desenvolvimento Local

### Comandos Úteis

```bash
# Desenvolvimento
npm start              # Inicia servidor de desenvolvimento
npm run dev            # Inicia e abre no navegador

# Testes
npm test               # Executa testes
npm run test:coverage  # Testes com cobertura

# Qualidade de Código
npm run lint           # Verifica linting
npm run format         # Formata código
npm run format:check   # Verifica formatação

# Build
npm run build          # Build de desenvolvimento
npm run build:prod     # Build de produção
```

### Estrutura de Pastas

Ao adicionar novos arquivos, siga a estrutura:

```
src/app/
├── components/        # Componentes reutilizáveis
├── pages/            # Páginas/rotas principais
├── services/         # Serviços
├── models/           # Interfaces e tipos
├── guards/           # Guards de roteamento
├── interceptors/     # HTTP interceptors
└── pipes/            # Pipes customizados
```

## 🤔 Dúvidas?

Se você tiver dúvidas sobre como contribuir:

1. Procure nas Issues existentes
2. Abra uma nova Issue com sua dúvida
3. Entre em contato com os mantenedores

## 🙏 Agradecimentos

Obrigado por dedicar seu tempo para contribuir com o Angular-Base! Cada contribuição, por menor que seja, é muito valorizada.

---

<div align="center">
  Feito com ❤️ pela comunidade
</div>
