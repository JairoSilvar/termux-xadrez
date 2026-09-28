XADREZ PRO v17.0.0 — TABULEIRO COMPLETO E PAINEL MÓVEL COMPACTO
Data: 28/09/2026
Base preservada: v16.0.0

OBJETIVO
Garantir que as oito fileiras do tabuleiro e todo o painel essencial apareçam na área visível do celular, inclusive no Firefox com barras dinâmicas, sem reduzir a largura normal do tabuleiro e sem remover recursos.

MUDANÇAS DA v17
- O jogo usa a altura real de window.visualViewport em navegadores móveis.
- Durante a partida, a página fica presa ao topo e não possui rolagem geral.
- O tabuleiro permanece quadrado, na largura máxima, mostrando as fileiras 8 até 1 e colunas a até h.
- Somente chat e menus suspensos possuem rolagem própria.
- Em partidas online, uma faixa fina mostra apenas cidade e tema.
- Identificadores técnicos permanecem escondidos.
- O botão Compartilhar abre o menu nativo do aparelho com link direto da sala.
- Sem Web Share, o convite é copiado; como último recurso, aparece para cópia manual.
- Links de convite reconhecem salas-cidade e salas criadas por jogadores.
- Se o nome estiver vazio, o convite aguarda o jogador informar o nome antes de entrar.
- Reagir, placar e histórico dividem a mesma faixa compacta.
- O chat recebe o espaço restante e pode ser aberto em tela ampliada.
- Frases rápidas continuam no botão ao lado da mensagem.
- Os cards dos dois jogadores permanecem visíveis.
- O PC conserva a organização aprovada na v16.

RECURSOS PRESERVADOS
Motor, regras, IA em cinco níveis, Bot vs Bot, P2P, espectadores, salas-cidade, salas criadas, rádio sincronizado, áudio, reações, frases rápidas, stand-up, histórico, FEN/PGN, temas, tabuleiros, peças, diagnóstico, PWA, Gold/GOD e DEV/TESTER.

CÓDIGOS
- 81=Nome: GOD.
- 82=Nome: DEV/TESTER.
Nenhum novo código foi adicionado.

VALIDAÇÃO EXECUTADA
- Sintaxe dos três scripts internos.
- Sintaxe do worker da IA, interface-v17.js e sw.js.
- Chaves CSS equilibradas.
- Nenhum ID HTML duplicado.
- Versão, build, cache, manifesto e arquivos carregados conferidos.
- Presença exclusiva dos códigos 81 e 82 conferida.

TESTES FÍSICOS RECOMENDADOS
- Firefox e Chrome no celular, com a barra do navegador aberta e recolhida.
- PWA instalada.
- Compartilhamento por WhatsApp, Google Mensagens e demais aplicativos disponíveis.
- Entrada pelo link como segundo jogador e como espectador.
- Microfone, rádio e P2P em dois aparelhos.
