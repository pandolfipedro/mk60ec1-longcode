# Validação local — 02/11/2026

Autoria do projeto: Pedro Pandolfi (@pandolfipedro).

## Automatizada

29 grupos de testes passaram com Node.js local e novamente após extrair o ZIP em um diretório limpo, executando npm run build, npm test e npm run check. Incluem:

- Hardwares H35/H45/H30/H31/H46 e comprimentos 18/19/20.
- Parsing de hexadecimal e Auto-Scan, espelhos e preservação de bits.
- Mapas VIN, whitelist e rotas de migração com decisões explícitas.
- Três presets, todas as combinações de câmbio e hardwares.
- Multilink/torção mudando apenas plataforma/servo e seu espelho.
- Manual/swap preservando o byte 16 e alterando somente o campo EDS conhecido.
- Sessão nova com preset/manual/eixo, sessão legada e rejeição de metadados inválidos.
- Créditos no HTML e presença dos dois botões de editor avançado.

## Navegador

- Jetta 2.5 manual/H31: aplicação em um clique e coding de 19 bytes.
- Jetta TSI DSG e Fusca TSI DSG: prévias aplicadas e plataformas distintas.
- Seletor manual e ação Aplicar câmbio: mesmo coding mantido quando EDS 2 já está correto.
- Atalho avançado abre e rola até os bytes; também retorna da aba Comparação para Funções.
- Sessão JSON e relatório TXT exportados com câmbio, preset e crédito de Pedro Pandolfi.
- Layout desktop e mobile 390 × 844; largura de documento 375 px, sem overflow horizontal.
- Nenhum erro de console observado nos fluxos verificados.

## Publicação

Build gera index.html e dist/index.html sem dependências npm. O workflow segue as ações documentadas do GitHub Pages. O envio ao GitHub e a execução do workflow hospedado ainda não ocorreram.

Não houve escrita no ABS nem validação física de veículos. Os presets permanecem bases editáveis e exigem conferência do conjunto instalado.
