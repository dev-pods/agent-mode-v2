## Etapa 1: Criando a Estrutura do Backend e do Frontend 🏗️

Chegou a hora de construir a fundação da sua aplicação! Nesta etapa, você usará o **Modo Agent do GitHub Copilot** para criar a estrutura inicial do backend (Node.js/Express) e do frontend (React/Vite).

### O que você deve criar

Sua aplicação deve ter duas pastas principais na raiz do repositório:

```
/backend
  package.json
  src/
    ...arquivos do servidor...

/frontend
  package.json
  src/
    ...arquivos do cliente...
```

### :keyboard: Atividade: Criar o Backend

1. Abra o **GitHub Copilot Chat** no VS Code (ou Codespaces).
2. Selecione o modo **Agent** no menu suspenso.
3. Cole o prompt abaixo e siga as instruções do Copilot:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=flat-square&logo=github%20copilot&labelColor=512a97&color=ecd8ff)
   >
   > ```prompt
   > Leia o arquivo de instruções do backend em .github/instructions/ e crie a estrutura
   > completa do backend conforme especificado. Certifique-se de criar o package.json
   > com todos os scripts necessários (start, dev, build, test).
   > ```

### :keyboard: Atividade: Criar o Frontend

1. Ainda no **GitHub Copilot Chat** com modo **Agent**, cole o prompt abaixo:

   > ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=flat-square&logo=github%20copilot&labelColor=512a97&color=ecd8ff)
   >
   > ```prompt
   > Leia o arquivo de instruções do frontend em .github/instructions/ e crie a estrutura
   > completa do frontend conforme especificado. Certifique-se de criar o package.json
   > com todos os scripts necessários (dev, build, lint, test).
   > ```

### :keyboard: Atividade: Fazer commit e push

Após criar as estruturas, faça commit e push das mudanças na branch `build-agent-mode`:

```bash
git add .
git commit -m "feat: adicionar estrutura de backend e frontend"
git push origin build-agent-mode
```

O GitHub Actions verificará automaticamente se as estruturas foram criadas corretamente.

<details>
<summary>Tendo problemas? 🤷</summary><br/>

Verifique se:
- A pasta `backend/` existe com um arquivo `package.json` dentro dela
- A pasta `frontend/` existe com um arquivo `package.json` dentro dela
- Cada pasta possui um diretório `src/` com pelo menos um arquivo de entrada

</details>
