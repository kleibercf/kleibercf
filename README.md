# Olá, sou Kleiber Ferreira

Este é meu portfólio de aplicações. Aqui compartilho os projetos que desenvolvo para resolver problemas do dia a dia.

## Projetos

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
