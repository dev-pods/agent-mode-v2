## Etapa 3: Criando Agents Customizados com o Modo Plan 🤖

Agora vamos explorar um dos recursos mais poderosos do GitHub Copilot: a criação de **agents customizados** a nível de repositório. Esses agents são especializados em tarefas específicas e ficam disponíveis para toda a equipe.

### O que você deve criar

Três arquivos de agent dentro da pasta `.github/agents/`:

```
.github/agents/
  test.agent.md        → Agent especializado em testes unitários
  review.agent.md      → Agent especializado em code review
  documentacao.agent.md → Agent especializado em documentação técnica
```

### :keyboard: Atividade: Usar o modo Plan para criar os agents

1. Abra o **GitHub Copilot Chat** no VS Code.
2. Selecione o modo **Agent** no menu suspenso.
3. Cole o prompt abaixo:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=flat-square&logo=github%20copilot&labelColor=512a97&color=ecd8ff)
   >
   > ```prompt
   > Planeje a criação dos seguintes agents customizados.
   > OBS: caso seja perguntado, informe que deseja criar os agents a nível de repositório: (.github/agents)
   >
   > 1° - Agent de test → Agent especializado em criação de testes unitários.
   > Analise funções, gere testes unitários, use mocks quando necessário, siga o padrão AAA
   > Backend → jest/supertest
   > Frontend → Vitest e React Testing library
   >
   > 2° - Agent de review → Agent especializado em code review.
   > Revise código, aponte problemas de performance, sugira melhorias de manutenabilidade e legibilidade.
   > Classifique cada achado com Critico/Importante/Sugestão. Verifique tratamento de erros.
   >
   > 3° - Agent de Documentação → Especialista em documentação técnica.
   > Gere documentação da api no formato Swagger. Mantenha linguagem clara e objetiva
   > e inclua exemplos de request/response para endpoints.
   > ```

4. Revise o plano proposto pelo Copilot e pressione **Continue** para executar.

### :keyboard: Atividade: Fazer commit e push

Após criar os agents, faça commit e push:

```bash
git add .
git commit -m "feat: adicionar agents customizados de test, review e documentação"
git push origin build-agent-mode
```

O GitHub Actions verificará se os três arquivos de agent existem no repositório.

<details>
<summary>Tendo problemas? 🤷</summary><br/>

Verifique se:
- Os arquivos estão criados exatamente em `.github/agents/`
- Os nomes dos arquivos são exatamente: `test.agent.md`, `review.agent.md` e `documentacao.agent.md`
- Cada arquivo tem conteúdo descrevendo o comportamento do agent

</details>
