XADREZ PRO v15.1.0 — CORREÇÕES DE ESTABILIDADE E DESEMPENHO

COMO PUBLICAR
1. Extraia o ZIP.
2. Copie todo o conteúdo extraído para a raiz do repositório ligado ao txadrez na Vercel.
3. Não crie uma pasta extra envolvendo index.html e api/.
4. Publique pelo fluxo normal do GitHub/Vercel.
5. Reabra o jogo e confirme “v15.1” na tela inicial.
6. Se uma versão anterior continuar aparecendo, feche e reabra o aplicativo e atualize a página para renovar o cache.

ARQUIVOS ALTERADOS NA v15.1
- index.html: sincronização P2P, IA, GOD, reações, rádio, logs e identificação da versão.
- interface-v15.js: identificação visual v15.1.
- manifest.json: descrição v15.1.0.
- sw.js: cache xp-sw-15.1.0-20260928.
- sw-v73.js: aviso explícito de arquivo histórico desativado.
- AUDIT.json: resultado das verificações automáticas.

CORREÇÕES PRINCIPAIS
- O ping P2P leva a lista compacta dos lances e reconstrói o histórico completo no aparelho remoto.
- Compatibilidade preservada com aparelhos antigos: quando a lista não existe, o jogo ainda sincroniza a posição e conserva o número remoto de jogadas.
- Logs de movimento mostram a notação e as casas de origem e destino.
- O campo ply do diagnóstico usa o histórico local ou o número conhecido do aparelho remoto.
- O estado do rádio no diagnóstico só aparece ligado quando há reprodução real e uma estação selecionada.
- A troca de estação encerra corretamente a transmissão anterior.
- Reações rápidas são agrupadas por 200 ms, transmitindo somente a última escolha do intervalo.
- A IA evita gerar listas completas de lances dentro da avaliação, usa quiescência mais curta e limita capturas analisadas.
- A avaliação separa material e posição; em finais, reduz o peso posicional para priorizar material.
- A chave da tabela de transposição inclui posição, turno, roque, en passant e profundidade.
- O GOD calcula somente na vez humana, usa orçamento superior ao da IA normal, mostra indicador de processamento e oferece uma sugestão segura se o cálculo exceder 2,5 segundos.
- Sugestões do GOD ficam vinculadas à posição exata e são recalculadas após desfazer um lance.
- A jogada da IA termina antes de iniciar uma nova análise GOD.
- Ao terminar uma partida Bot vs Bot, os cards deixam imediatamente o estado “Processando...”.

INTERFACE PRESERVADA
- Tabuleiro no maior tamanho possível no computador e no celular.
- Painel líquido, sem rolagem externa durante a partida.
- Chat ocupa o espaço restante do painel.
- Seis botões superiores uniformes, placar discreto e painéis sobrepostos de opções, reações e frases.
- Prévia de áudio flutuante, sem deslocar os cards.
- Configurações responsivas, prévias visuais, rádios em lista e diagnóstico com cópia, download e compartilhamento.

CONFIGURAÇÃO VERCEL
Mantenha as variáveis existentes do projeto. O registro de salas usa KV_REST_API_URL + KV_REST_API_TOKEN ou UPSTASH_REDIS_REST_URL + UPSTASH_REDIS_REST_TOKEN. Nunca coloque tokens nos arquivos do jogo.

VALIDAÇÃO EXECUTADA
- Sintaxe de todos os scripts inline, interface-v15.js, sw.js e worker da IA.
- Busca de IDs duplicados no HTML.
- Renderização no navegador em 1366x768 e 392x735.
- Tabuleiro, painel, chat e ausência de rolagem externa.
- Console do navegador sem erros ou avisos durante a partida local.

VALIDAÇÃO NECESSÁRIA APÓS PUBLICAR
- Partida P2P real entre dois aparelhos v15.1, incluindo reconexão e desfazer.
- Compatibilidade entre v15.1 e uma versão anterior.
- Tempo da IA e do GOD em aparelhos reais de diferentes capacidades.
- Microfone, compartilhamento nativo, instalação PWA e transmissões de rádio.
- Teste de stress DEV/TESTER com 500 ciclos.

PRESERVAÇÃO
O motor de regras, os modos de jogo, salas online, tutorial, histórico, temas, peças, estilos, conquistas, áudio, rádio, diagnóstico, PWA e demais recursos permanecem no pacote. Nenhum recurso foi intencionalmente removido.

BASE
Pacote XadrezPro-v15.0.0, SHA-256 931FF16DB3F04EBA9806D0C1F7D0EF8A85859B0D055AC524574A4A6A0D6B77C3.

Este pacote não foi enviado ao GitHub nem publicado automaticamente.
