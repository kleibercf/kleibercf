# Olá, sou Kleiber Ferreira

Este é meu portfólio de aplicações. Aqui compartilho os projetos que desenvolvo para resolver problemas do dia a dia.

## Projetos

[Sistema de Ponto](#sistema-de-ponto) · [Sistema de Estoque](#sistema-de-estoque) · [Gerenciador de Discos](#gerenciador-de-discos)

### Sistema de Ponto

Desenvolvi uma aplicação web para registrar jornadas de trabalho e ajudar o RH a acompanhar a frequência e fechar as folhas de ponto.

- **Registro de jornada** — marcação de entradas e saídas e consulta ao histórico.
- **Rotina do RH** — gestão de funcionários, análise de justificativas e acompanhamento do banco de horas.
- **Fechamento de períodos** — conferência das marcações e geração de folhas de ponto em PDF.

Atuei na arquitetura e no desenvolvimento da aplicação, da interface à persistência dos registros e à geração dos relatórios.

**Tecnologias** — Python, SQLite, JavaScript, HTML e CSS.

#### Demonstração com dados fictícios

**Meu ponto** — O funcionário registra a jornada e acompanha seu histórico e as pendências.

![Tela Meu ponto com registros de entrada, intervalo e histórico de marcações](imagens/sistema-de-ponto/meu-ponto.png)

**Validação de justificativas** — O RH analisa solicitações de atraso ou marcação faltante e decide se deve validar, devolver ou recusar.

![Tela de validação com três justificativas fictícias aguardando análise do RH](imagens/sistema-de-ponto/validacao-de-justificativas.png)

**Fechamento do período** — O RH confere horas previstas, trabalhadas e saldos antes de finalizar as folhas e exportá-las em PDF.

![Relatório de ponto com duas folhas finalizadas, uma pendente e opções de exportação em PDF](imagens/sistema-de-ponto/fechamento-do-periodo.png)

**Banco de horas** — O RH acompanha os saldos por funcionário, os créditos e débitos lançados e o valor a pagar em folha.

![Tela de Banco de horas com saldos por funcionário e um lançamento de crédito](imagens/sistema-de-ponto/banco-de-horas.png)

**Folha finalizada** — A folha individual reúne as marcações diárias, as horas previstas e trabalhadas e o saldo do período após o fechamento.

![Folha individual finalizada com cinco dias de marcações e saldo positivo de uma hora](imagens/sistema-de-ponto/folha-finalizada.png)

**Relatório gerado em PDF** — A folha exportada reúne as marcações, o resumo de horas e os campos de assinatura.

<img src="imagens/sistema-de-ponto/relatorio-gerado.png" width="680" alt="Folha de ponto exportada em PDF com dados fictícios, tabela de marcações, resumo e campos de assinatura">

### Sistema de Estoque

Desenvolvi uma central web para organizar o inventário por filial, da identificação dos produtos à conferência dos saldos.

- **Contagem Diária** — importação de listas em CSV, contagem cega com leitura de QR e aprovação dos resultados. Quando há divergências, o responsável pode solicitar a recontagem apenas dos itens afetados.
- **Balanço de Estoque** — contagem por rua e prateleira, consolidação das rodadas e exportação em CSV para o ERP Solution.
- **Etiquetas QR** — geração de folhas A4 a partir de CSV, com código, identificação e alocação do produto.

Atuei na arquitetura e no desenvolvimento da interface, da API e dos fluxos de contagem e aprovação.

**Tecnologias** — Node.js, SQLite, JavaScript, HTML e CSS.

#### Demonstração do estoque com dados fictícios

**Central de operações** — acesso aos três módulos do sistema.

![Central de operações com Contagem Diária, Balanço de Estoque e Etiquetas QR](imagens/sistema-de-estoque/central-de-operacoes.png)

**Contagem Diária** — o estoquista registra as quantidades após identificar os produtos pelo QR. O saldo de referência fica oculto durante a coleta.

![Contagem cega em andamento, com quatro produtos contados e dois pendentes](imagens/sistema-de-estoque/contagem-diaria.png)

**Balanço de Estoque** — o painel mostra a proporção de itens conformes e divergentes, com filtros por balanço, linha de produto, funcionário, rua e alocação.

![Painel do balanço com oito itens consolidados, seis conformes e dois divergentes](imagens/sistema-de-estoque/dashboard-do-balanco.png)

**Etiquetas QR** — prévia da folha A4 com os códigos, as descrições e as posições dos itens.

![Oito etiquetas de demonstração com QR, identificação do produto e alocação](imagens/sistema-de-estoque/etiquetas-qr.png)

**Relatório de contagem** — o relatório gerado após a aprovação compara as quantidades contadas com os saldos do sistema e destaca as diferenças.

![Relatório gerado pelo sistema para uma contagem aprovada de seis itens, com duas divergências](imagens/sistema-de-estoque/relatorio-de-contagem.png)

### Gerenciador de Discos

Desenvolvi uma ferramenta de terminal para formatar pendrives e gerenciar discos e partições no Windows. A ferramenta reúne operações de armazenamento em um menu e mostra o dispositivo e o efeito da ação antes de pedir confirmação.

- **Consulta** — lista discos e partições e ajuda a distinguir unidades USB do disco do sistema.
- **Formatação e particionamento** — oferece NTFS, exFAT e FAT32 conforme o tamanho do volume e permite criar, redimensionar ou excluir partições.
- **Controle de operações** — protege discos do sistema, exige confirmação específica e revalida a identidade e o layout do disco antes de alterar o dispositivo.

A suíte inclui 33 verificações com discos simulados, incluindo cancelamento, troca de dispositivo e registro de falhas.

**Tecnologias** — Windows PowerShell 5.1 e módulo Storage do Windows.
