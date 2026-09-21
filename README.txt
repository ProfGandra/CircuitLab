CircuitLab v0.6 — Matrícula e crachá revisado

Alterações principais desta versão:
- Tela inicial alterada de “Criar credencial” para “Matrícula do aluno”.
- Subtítulo atualizado para: “Um jogo de Análise, cálculo e validação de circuitos.”
- A figurinha do instrutor foi removida da tela de matrícula.
- A área direita da tela inicial agora exibe uma prévia dinâmica do crachá do aluno.
- O crachá é atualizado conforme o nome e o gênero são selecionados.
- Ordem visual obrigatória do crachá:
  1. Logotipo/identificação SENAI-SP em vermelho sobre fundo branco;
  2. Avatar genérico;
  3. Nome do aluno;
  4. Código de barras genérico.
- Gênero mantém as opções Masculino, Feminino e Prefiro não dizer.
- A mesma organização do crachá é usada na versão compacta do HUD.
- Permanecem pontuação acumulada, cheatcode, níveis, sorteio de valores e multímetro interativo da v0.5.

Para testar: abra index.html em um navegador moderno.


v0.6.1
- Melhorado contraste da lista de Gênero.
- Avatares masculino, feminino e neutro redesenhados sem ferramentas e com óculos de proteção.
- Avatar 'Prefiro não dizer' agora é humano neutro.
- Removido glifo/emoji do título Matrícula do aluno.


v0.6.2
- Óculos de proteção dos avatares substituídos por óculos comuns.
- Tela de matrícula não exibe mais a credencial do último aluno salva localmente.
- O HUD da tela inicial começa neutro; a credencial aparece após matrícula/restauração durante o jogo.


v0.7 — Revisão estrutural dos diagramas
- Diagramas dos níveis 2, 3, 4, 7, 8 e 10 reconstruídos a partir de caminhos elétricos contínuos.
- Nível 2: R1, R2 e R3 realmente em série entre A e B.
- Nível 3: R1 e R2 agora compartilham exatamente os mesmos nós A e B.
- Nível 4/10: topologia A — R1 — (R2 || R3) — R4 — B corrigida.
- Nível 7: malha fechada e indicação I=? reposicionada para não sobrepor R1.
- Nível 8: malha KVL fechada e contínua.
- Crachá agora utiliza o arquivo gráfico do logotipo SENAI-SP fornecido pelo usuário.
- Campo Nome com fundo escuro e texto claro.
- Tela de conclusão de nível utiliza a nova figurinha de sinal de jóia.


v0.8 — Multímetro prático
- Reintroduzido uso prático do multímetro nos níveis 6 a 10.
- Pontas preta e vermelha são arrastáveis.
- A medição só é aceita quando a função do multímetro e os dois pontos de conexão estão corretos.
- Nível 6: medição de resistência em componente desenergizado.
- Nível 7: tensão em paralelo e corrente em série.
- Nível 8: medição de queda de tensão para validar KVL.
- Nível 9: medição de corrente de ramo para validar a lei dos nós.
- Nível 10: medições finais de tensão e corrente com menos orientação.


v0.8.1 — Pontas de prova
- Pontas redesenhadas com corpo, proteção, pescoço e agulha metálica longa, inspiradas na referência fornecida.
- Validação elétrica agora ocorre pela extremidade metálica da ponta de prova.
- A parte plástica da ponta não aciona mais o ponto de medição.
- Snap visual ajustado para encostar a agulha metálica no nó de medição.


v0.9 — Parte 2: Capacitores em CC e Osciloscópio
Níveis 1–10 = Parte 1, circuitos resistivos.
Níveis 11–20 = Parte 2, capacitores em CC.
Inclui capacitância, associações, medição, RC, constante de tempo, treinamento de osciloscópio, carga, descarga e laboratório final.


v0.9.2 — Correção definitiva do cheatcode
- Novo formato CL2 com Base64 URL-safe.
- Restauração recompõe automaticamente o padding Base64.
- Codificação/decodificação UTF-8 robusta com TextEncoder/TextDecoder.
- Cheatcodes agora suportam corretamente os 20 níveis.
- Validação de integridade mantida por checksum.
- Códigos antigos CL- não são mais utilizados; a nova versão gera e restaura CL2-.

Código de teste Nível 11:
CL2-eyJ2IjoyLCJuIjoiQWx1bm8gVGVzdGUiLCJnIjoiTiIsInMiOjI1MDAsImwiOjEwLCJkIjoiMjAyNi0wOC0xNFQxMjowMDowMC4wMDBaIiwiciI6IkNBUFRFU1QxIn0-1INNGOK

Código de teste Nível 17:
CL2-eyJ2IjoyLCJuIjoiQWx1bm8gVGVzdGUiLCJnIjoiTiIsInMiOjM4MDAsImwiOjE2LCJkIjoiMjAyNi0wOC0xNFQxMjowNTowMC4wMDBaIiwiciI6Ik9TQ1RFU1QxIn0-1TE1EG


v0.9.3 — Cheatcode funcional e JavaScript validado
- Corrigido fechamento do renderer do nível 10, que impedia o script da Parte 2 de carregar corretamente.
- Removido fragmento obsoleto da antiga função de cheatcode.
- Novo formato CL3 com UTF-8, Base64 URL-safe e checksum.
- Progressão liberada corretamente até o nível 20.
- JavaScript validado com Node.js (`node --check`).

Código para liberar Nível 11:
CL3-eyJ2IjozLCJuIjoiQWx1bm8gVGVzdGUiLCJnIjoiTiIsInMiOjI1MDAsImwiOjEwLCJkIjoiMjAyNi0wOC0xNFQxMjowMDowMC4wMDBaIiwiciI6IkNBUFRFU1QzIn0-1LZD4JZ

Código para liberar Nível 17:
CL3-eyJ2IjozLCJuIjoiQWx1bm8gVGVzdGUiLCJnIjoiTiIsInMiOjM4MDAsImwiOjE2LCJkIjoiMjAyNi0wOC0xNFQxMjowMDowMC4wMDBaIiwiciI6Ik9TQ1RFU1QzIn0-DFLAXY

Código para liberar Nível 20:
CL3-eyJ2IjozLCJuIjoiQWx1bm8gVGVzdGUiLCJnIjoiTiIsInMiOjUwMDAsImwiOjE5LCJkIjoiMjAyNi0wOC0xNFQxMjowMDowMC4wMDBaIiwiciI6IlJDVEVTVDAzIn0-15J1O9X


v0.9.4 — Osciloscópio interativo
- VOLTS/DIV agora altera realmente a escala vertical do traçado.
- TIME/DIV altera a janela temporal e a escala horizontal.
- Trigger reposiciona a aquisição pelo cruzamento do nível selecionado.
- RUN/STOP passa a ter estado funcional.
- Escalas incluem µs, ms e s/div.
- A linha de 1τ muda de posição conforme TIME/DIV e pode sair da tela.
- Quando VOLTS/DIV é insuficiente, o traço é recortado e aparece aviso de sinal fora da escala.
- A curva continua sendo calculada a partir dos valores sorteados de R, C e V.
- JavaScript validado com Node.js antes da entrega.


v1.0 — Parte 3: Transistores (Níveis 21–30)
21 Introdução aos transistores
22 BJT NPN e PNP
23 Junções e polarização
24 Correntes IB, IC e IE
25 Ganho β
26 Corte, ativa e saturação
27 Transistor como chave
28 Polarização CC
29 Medição/diagnóstico com teste de diodo
30 Laboratório de multivibrador astável / pisca-LED

Nível 30:
- R1 e R2 variáveis em tempo real.
- LEDs alternam conforme o estado calculado dos BJTs.
- t1, t2, período, frequência e duty cycle calculados pelas constantes RC.
- Osciloscópio mostra coletor Q1, coletor Q2 e tensão de base/capacitor.
- O modelo NÃO usa ondas quadradas digitais ideais.
- Tensões dos capacitores/bases seguem curvas exponenciais.
- Coletores são limitados por corte e VCE(sat), refletindo a saturação do transistor.
- Alterar R1/R2 muda simultaneamente temporização, LEDs e traçados.
- Progressão/cheatcode ampliados para 30 níveis.
- JavaScript validado com Node.js.


v1.0.1 — Assinatura visual
- Figurinha do instrutor adicionada no canto inferior direito em todas as telas internas.
- A figurinha NÃO aparece na página inicial/matrícula.
- Texto abaixo da figurinha: "Desenvolvido por DGandra - 2026".
- Elemento usa tamanho responsivo e pointer-events:none para não bloquear botões, navegação ou conteúdo.
- Rodapé ajustado para evitar sobreposição.


v1.0.2 — Figurinha com fundo transparente
- Utilizada exatamente a figurinha original fornecida pelo usuário.
- Removido somente o fundo branco externo, preservando a arte original.
- Asset `assets/dgandra_instrutor.png` substituído pela versão PNG transparente.
- Mantida no canto inferior direito das telas internas.
- Mantido o crédito: "Desenvolvido por DGandra - 2026".
- A figurinha continua oculta na página inicial/matrícula.
