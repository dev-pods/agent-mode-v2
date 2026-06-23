## Etapa 4: Gerando Testes Unitários com o Agent de Testes 🧪

Com seus agents criados, é hora de colocá-los em ação! Nesta etapa, você usará o **agent de testes** para gerar testes unitários para a aplicação.

### O que será verificado

O GitHub Actions irá:
1. Verificar a existência de arquivos de teste (`*.test.*` ou `*.spec.*`) no backend e no frontend
2. Executar `npm test` no **backend** e validar que os testes passam
3. Executar `npm test` no **frontend** e validar que os testes passam

### :keyboard: Atividade: Usar o agent de testes

1. Abra o **GitHub Copilot Chat** no VS Code.
2. Selecione o modo **Agent** e depois escolha o agent **@test** (ou o nome que você deu ao agent de testes).
3. Cole o prompt abaixo:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=flat-square&logo=github%20copilot&labelColor=512a97&color=ecd8ff)
   >
   > ```prompt
   > Gere testes completos para o arquivo de documentos cobrindo cenários de
   > validação de sucesso, cpf inválido, matrícula inexistente
   > ```

4. Revise os testes gerados e faça ajustes se necessário.

### :keyboard: Atividade: Validar testes localmente

Execute os testes localmente antes de fazer commit:

**Backend:**
```bash
cd backend
npm test
```

**Frontend:**
```bash
cd frontend
npm test
```

### :keyboard: Atividade: Fazer commit e push

```bash
git add .
git commit -m "test: adicionar testes unitários com agent de testes"
git push origin build-agent-mode
```

O GitHub Actions executará os testes automaticamente e reportará os resultados.

<details>
<summary>Tendo problemas? 🤷</summary><br/>

Verifique se:
- Existem arquivos de teste com extensão `.test.js`, `.test.ts`, `.spec.js` ou `.spec.ts`
- O script `test` está definido no `package.json` de cada projeto
- Os testes passam localmente antes de fazer push

</details>
