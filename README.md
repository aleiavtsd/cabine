# Campaign OS

Site estático de arquivo único (`index.html`). Não precisa de build nem de dependências.

## Publicar na Vercel

### Opção A: pelo GitHub (recomendada)
1. Crie um repositório novo no GitHub e envie os arquivos desta pasta (botão "Add file > Upload files").
2. Na Vercel, clique em "Add New > Project" e importe o repositório.
3. Deixe "Framework Preset" como **Other**, sem comando de build e sem pasta de saída. Clique em **Deploy**.
4. Em cerca de um minuto você recebe um link `nome.vercel.app`. Cada novo envio ao GitHub republica sozinho.

### Opção B: pelo terminal
```
npm i -g vercel
cd campaign-os-vercel
vercel --prod
```
Responda às perguntas com os padrões (sem framework, pasta atual).

## Depois de publicar
- Abra o link numa janela anônima para confirmar que abre sem login.
- Em Settings > Domains, você pode ligar um domínio próprio.
- Os dados de cada pessoa ficam no navegador dela (localStorage). Para login e banco de dados, use o Prompt 2 do arquivo de prompts do Lovable ou adicione um backend.
