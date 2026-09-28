XADREZ PRO v16.0.0 — INTERFACE LÍQUIDA PARA PC E CELULAR
Data: 28/09/2026
Base preservada: v15.1.1

OBJETIVO
A versão 16 reorganiza a apresentação do jogo sem reduzir o protagonismo do tabuleiro e sem alterar as regras, o motor, o P2P ou os códigos secretos existentes.

PRINCIPAIS MUDANÇAS
- Tabuleiro continua ocupando o maior espaço possível no PC e no celular.
- Painel lateral do PC acompanha exatamente a altura do tabuleiro.
- Chat absorve o espaço vertical restante e deixa de criar área vazia abaixo do último card.
- Cabeçalho possui seis controles uniformes e responsivos.
- Placar de vitórias foi mantido como informação fina e discreta.
- Reações usam uma superfície sólida e legível; no celular abrem em painel suspenso com botão para fechar.
- Frases rápidas permanecem compactas no PC e viram um único botão junto à mensagem no celular.
- Prévia de áudio abre por cima do conteúdo, sem deslocar os cards.
- Menus Opções, Reações e Frases rápidas possuem fechamento explícito no celular.
- Peças capturadas ficaram mais legíveis sem aumentar os cards.
- Apenas o bot que está calculando mostra “Pensando...”.
- Botão flutuante DEV/TESTER não cobre o tabuleiro durante a partida; o acesso permanece em Opções.
- Compartilhamento de diagnóstico tenta anexar o TXT pelo compartilhamento nativo e mantém cópia/download como alternativa.

CÓDIGOS MANTIDOS
- 81=Nome: modo GOD.
- 82=Nome: modo DEV/TESTER.
- Nenhum código 83, 84, 85 ou 86 foi implementado.

ARQUIVOS DA CAMADA VISUAL
- interface-v16.css
- interface-v16.js

VALIDAÇÃO EXECUTADA
- Sintaxe dos scripts internos, worker, interface-v16.js e service worker.
- IDs duplicados: nenhum.
- Referências de versão, build, manifesto e cache conferidas.
- Presença exclusiva dos códigos 81 e 82 conferida.

VALIDAÇÃO NECESSÁRIA NO APARELHO
- Conferência visual nas dimensões reais de PC e celular.
- Microfone e prévia de áudio.
- Compartilhamento nativo e download TXT.
- Rádio, PWA e menus suspensos.
- Partida P2P em dois aparelhos.

INSTALAÇÃO
Publique todo o conteúdo desta pasta na raiz do projeto Vercel. Depois da publicação, feche e reabra o aplicativo ou recarregue sem cache para ativar o service worker v16.
