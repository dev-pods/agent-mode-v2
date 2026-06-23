## Etapa 2: Instalando Dependências e Validando a Aplicação ⚙️

Ótimo trabalho na criação das estruturas! Agora vamos garantir que sua aplicação consegue instalar as dependências e ser executada sem erros.

### O que será verificado

O GitHub Actions irá:
1. Executar `npm ci` no **backend** — instalar dependências do servidor
2. Executar `npm ci` no **frontend** — instalar dependências do cliente
3. Executar `npm run build` em ambos — validar que o código compila sem erros

### :keyboard: Atividade: Testar localmente

Antes de fazer commit, teste sua aplicação localmente para garantir que tudo funciona:

**Backend:**
```bash
cd backend
npm install
npm run dev
```

**Frontend:**
```bash
cd frontend
npm install
npm run dev
```

> [!TIP]
> Se estiver usando Codespaces, abra dois terminais — um para o backend e outro para o frontend.

### :keyboard: Atividade: Corrigir problemas com o Copilot

Se encontrar erros ao tentar instalar ou executar, use o **Modo Agent** para ajudar:

> ![Static Badge](https://img.shields.io/badge/-Prompt-text?style=flat-square&logo=github%20copilot&labelColor=512a97&color=ecd8ff)
>
> ```prompt
> Ao tentar executar npm install no backend/frontend, estou recebendo o seguinte erro: [cole o erro aqui].
> Por favor, analise e corrija o problema.
> ```

### :keyboard: Atividade: Fazer commit e push

Após validar que a aplicação funciona localmente, faça commit e push:

```bash
git add .
git commit -m "fix: corrigir dependências e configuração de build"
git push origin build-agent-mode
```

O GitHub Actions tentará instalar as dependências e realizar o build para validar que tudo está funcionando.

<details>
<summary>Tendo problemas? 🤷</summary><br/>

Verifique se:
- O `package.json` do backend tem o script `build` definido (pode ser apenas `"build": "echo ok"` se não for necessário compilar)
- O `package.json` do frontend tem o script `build` definido (geralmente `vite build`)
- Não há dependências faltando ou conflitos de versão

</details>
