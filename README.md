# LR Team, Rei do Personal

App do campeonato de futevôlei. Página estática (`index.html`) mais uma API (`api/state.js`) que guarda os placares em um Redis da Upstash.

## Publicar na Vercel

1. Crie um repositório no GitHub e suba todos os arquivos desta pasta.
2. Na Vercel, clique em **Add New > Project**, escolha o repositório e clique em **Deploy**. Pode deixar todas as configurações como estão.
3. Quando terminar, abra o projeto na Vercel, vá em **Storage** (ou **Marketplace**) e adicione **Upstash > Redis**, plano gratuito. Conecte ao projeto. A Vercel cria sozinha as variáveis de ambiente do banco.
4. Vá em **Deployments**, abra o menu do último deploy e clique em **Redeploy**, para a API enxergar o banco.
5. Abra o link `seu-projeto.vercel.app`. O topo deve mostrar "Ao vivo".

## Usar

Qualquer pessoa com o link vê a tabela e lança placares. A tela atualiza sozinha a cada poucos segundos.

## Deixar o campeonato zerado

No painel da Upstash, abra o banco, entre em **Data Browser** e apague a chave `lrteam:campeonato`.
