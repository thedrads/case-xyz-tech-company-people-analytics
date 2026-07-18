# Como contribuir

Obrigado pelo interesse em contribuir.

## Fluxo recomendado

1. Crie um fork do repositório.
2. Crie uma branch a partir de `main`.
3. Faça alterações pequenas e focadas.
4. Execute o notebook integralmente em uma sessão limpa.
5. Abra um pull request descrevendo objetivo, alterações e validações.

## Convenção de branches

- `feat/descricao-curta`: nova funcionalidade;
- `fix/descricao-curta`: correção;
- `docs/descricao-curta`: documentação;
- `chore/descricao-curta`: manutenção.

## Commits

Use mensagens objetivas no imperativo, preferencialmente seguindo Conventional Commits:

```text
feat: adiciona nova visualização
fix: corrige cálculo do percentual
 docs: melhora documentação da metodologia
```

## Padrões de código

- Siga a PEP 8.
- Use nomes descritivos.
- Inclua type hints em funções.
- Documente decisões de negócio, não o óbvio.
- Evite células com múltiplas responsabilidades.
- Não oculte avisos globalmente sem justificativa.

## Qualidade do notebook

Antes do pull request:

- reinicie a sessão;
- execute todas as células em ordem;
- confirme ausência de erros;
- valide que tabelas e gráficos foram renderizados;
- confira se arquivos exportados foram recriados;
- remova dados sensíveis e saídas temporárias.

## Pull requests

O pull request deve informar:

- problema ou objetivo;
- alterações realizadas;
- forma de validação;
- impactos nos resultados;
- screenshots quando houver mudança visual.
