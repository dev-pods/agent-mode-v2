## Etapa 5: Atualizando a Documentação com o Agent de Docs 📝

Parabéns por chegar até aqui! Na etapa final, você usará o **agent de documentação** para atualizar os READMEs do backend e do frontend com informações completas e úteis.

### O que será verificado

O GitHub Actions irá verificar se:
1. Existe `backend/README.md` com conteúdo relevante
2. Existe `frontend/README.md` com conteúdo relevante
3. Os READMEs contêm seções obrigatórias:
   - **Como rodar** (ou "Como executar", "Getting Started")
   - **Descrição** (ou "Sobre", "About")
   - **Dados de teste** (ou "Mocks", "Exemplos")

### :keyboard: Atividade: Usar o agent de documentação

1. Abra o **GitHub Copilot Chat** no VS Code.
2. Selecione o modo **Agent** e escolha o agent **@documentacao**.
3. Cole o prompt abaixo:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=flat-square&logo=github%20copilot&labelColor=512a97&color=ecd8ff)
   >
   > ```prompt
   > Atualize as documentações dos readmes do front e do back com informações sobre
   > como rodar, descritivo breve do projeto e possíveis dados para teste com base
   > nos mocks. Utilize #runSubagent para paralelizar as atualizações.
   > ```

4. Revise os READMEs atualizados para garantir que estão completos e corretos.

### :keyboard: Atividade: Fazer commit e push

```bash
git add .
git commit -m "docs: atualizar README do backend e frontend com agent de documentação"
git push origin build-agent-mode
```

O GitHub Actions verificará o conteúdo dos READMEs e confirmará a conclusão do curso.

---

## 🎉 Parabéns!

Ao concluir esta etapa, você terá:
- ✅ Construído uma aplicação completa com backend e frontend
- ✅ Criado agents customizados de teste, review e documentação
- ✅ Gerado testes unitários automaticamente com IA
- ✅ Documentado sua aplicação com ajuda do Copilot

Você está pronto para usar o **GitHub Copilot no modo Agent** em seus projetos do dia a dia! 🚀

<details>
<summary>Tendo problemas? 🤷</summary><br/>

Verifique se:
- Os arquivos `README.md` existem em `backend/` e `frontend/`
- Cada README contém ao menos uma seção sobre como rodar a aplicação
- Cada README contém uma descrição do projeto
- Cada README menciona dados de teste ou mocks disponíveis

</details>
