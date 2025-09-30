# Aplicação da empresa — Visão Geral

**Data:** 30/09/2025
**Autor:** Alex

Proponho dois nomes simples:
- ARTE(aplicativo de registos e trabalho eficiente) — porque o trabalho bem feito também é arte sem falar que podemos chamar os colaboradores de artistas, igual o sr. Paulo utiliza muitas vezez(me lembro disso nos meus primeiros dias na pcarnes).
ou
- PCarnes App — direto e reconhecível por todos.
---

## 1) Ideia em poucas palavras

- Vamos ter uma aplicação única (o ponto de entrada) com login, que depois de autenticado mostra botões para módulos por departamento na lateral e un feed central igual um social app como facebook.
- Cada colaborador vê só o que precisa dos módulos. Dentro de cada módulo, existem papéis simples (por exemplo: operador, responsável, admin).
- Tudo o que acontece fica registado: quem fez, quando, em que linha/área e que lote estava a ser trabalhado.
- Haverá ecrãs(dashboards) com informação ao vivo: na administração e em alguns televisores na fábrica (por exemplo, na cozinha), para todos perceberem como está o dia.
- O sistema cresce por etapas: começamos pelo que não temos ainda no SARA e vamos adicionando módulos até cobrir todos os departamentos já existentes no SARA.

---

## 2) Como será usar no dia a dia

1. O colaborador entra na aplicação, faz login e escolhe o seu módulo (ex.: Armazém, Produção, Qualidade) ou consulta o feed de noticias.
2. O módulo mostra tarefas simples, formulários adaptados ao contexto.
3. Ao registar, guardamos quem fez, quando, onde e o que. Podemos anexar fotografias e documentos.
4. Na administração, um ecrã mostra o que já foi produzido hoje, paragens e motivos, encomendas prontas a sair, incidentes, leituras de controlo e outras informações úteis.
5. Se a internet falhar, a operação continua na rede interna e os registos ficam em fila para seguirem quando a ligação voltar.

---

## 3) Departamentos e módulos (o que já temos e o que vamos ter)

> Em todos os módulos: registo completo, anexos (fotos/PDF), pesquisa por período, exportação, e campo para observações.

### 3.1. Logística e Armazém

**Armazém** — já usamos hoje, vamos melhorar
- Entradas e saídas de materiais de escritório, temperos e consumíveis.
- Pedidos internos (ja funcional mas como uma pequena alteraçao, possibilidade de marcar como entregue e registar o movimento diretamente no pedido).
- Leitura de códigos de barra para consulta da situação daquele artigo ou para transferencias ou saidas.
- Lista diária de necessidades para a produção que é calculada automaticamente assim que inserimos uma produção na folha de produção.

*O que podemos escolher para ver nos dashboards*
- Pedidos preparados a tempo, diferenças de stock, tempo médio de preparação.

*Sugestões*
- Canal de alertas diretamente no módulo (notificações push nos telemoveis dos colaboradores desse departamento dos pedidos internos ou stocks baixos).
- Um sistema que obriga a fazer inventários aleatorios ou definidos de x em x tempo, para não parar tudo de uma vez.

**Expedição — cliente H3** — já existe renovado
- Encomendas por destino, visão diária, lotes, verificação de execução.
- Rotas com lojas e motoristas; aviso de encomendas duplicadas e decisão do responsável.

*O que podemos escolher para ver nos dashboards*
- Entregas a tempo, erros por duplicação, rotas concluídas.

*Sugestões*
- Prova de entrega com fotografia e assinatura.
- Pequena lista de verificação de temperatura e condições por rota.
- Registo de combustiveis.
- Avarias, datas de manutenção e outros documentos.

**Expedição — geral**
- Registos do que sai: produto, quantidade, destino, transportador, temperaturas e condições de transporte.
- Libertação do produto quando cumpre os requisitos IFS (por exemplo, controlo de metais e rótulos).

*O que podemos escolher para ver nos dashboards*
- Saídas por hora, produto e cliente, ocorrências na expedição.

**Entradas**
- Todas as entradas: consumíveis de escritório e matéria‑prima (carne embalada ou ao natural, animais para desmancha).
- Fornecedor, transporte, produto, documentos/fotos, quantidades, pontos de segurança alimentar, validades e lotes, decisão (aprovado/rejeitado parcial ou total), assinaturas.

*O que podemos escolher para ver nos dashboards*
- Hora das receções, rejeições por fornecedor/produto e motivos.

*Sugestões*
- Aviso de chegada do camião para acelerar o processo.

**Devoluções**
- Formulário simples para devoluções: origem, motivo, estado do produto, temperatura, fotos e destino final (retornar, destruir, reprocessar).
- Mantemos a ligação ao lote para rastrear.

*O que podemos escolher para ver nos dashboards*
- As últimas devoluções.

---

### 3.2. Produção

> Podemos incluir aqui os 3 departamentos que temos no SARA: **Desmancha**, **Fatiados** e **Transformação(em vez de produção)**. Assim os ecrãs e os registos ficam feitos à medida.

**Desmancha**
- Lista de peças.
- Registos de detetor de metais.
- Registos de mudança de tábuas.
- Análise de gordura se a nova maquina ficar para o lado da desmancha em vez da frente da picadora.

*O que podemos escolher para ver nos dashboards*
- O que se desmancha no momento e um historico dar ultimas desmanchas com detalhes das horas e pesos.

**Fatiados**
- Registos de temperaturas, estanquicidade e gas, detetores de metais.
- Registos de falta de gás nas maquinas de fechar.

*O que podemos escolher para ver nos dashboards*
- Falhas de estanquicidade, temperaturas, valores de gás fora do esperado, rejeições, falta de gás.

*Sugestões*
- Avisos quando os valores começam a aproximar‑se dos limites, para agir antes de falhar.

**Transformação**
- Etapas: picagem, mistura, formatação e embalagem.
- Temperaturas estanquicidade e gas, detetores de metais.
- Limpeza de facas das picadoras.
- Analisador de gordura (hoje no SARA está aqui; mais tarde pode passar para Desmancha).

*O que podemos escolher para ver nos dashboards*
- Falhas de estanquicidade, temperaturas, valores de gás fora do esperado, rejeições, falta de gás, historico das limpezas das facas.

**Cozedura**
- Programas por equipamento, produto, espécie e pesos.
- Leitura das pilhas com gráficos e verificação automática de tempo e temperatura de cozedura/esfriamento.
- Relatório final em PDF.

*O que podemos escolher para ver nos dashboards*
- Ciclos conformes, tempos de arrefecimento, falhas por equipamento.

**Folha de Produção** — já renovada
- Receitas de produtos compostos (carne, água, ingredientes, cuvetes, separadores, filme, etiquetas).
- Explicação por fase para o operador.
- Ordens de produção visíveis nas linhas; o operador marca quando termina e pode deixar observações.
- Necessidades de materiais visíveis para o Armazém.

*O que podemos escolher para ver nos dashboards*
- Ordens feitas ou não feitas, diferenças entre o previsto e o realizado, consumos para cada materia prima, ingrediente ou material de embalagem.

---

### 3.3. Qualidade e Segurança Alimentar

**Qualidade**
- Pre-operativa.
- Materiais quebráveis.
- Formação e avaliação dos colaboradores.
- Testes rápidos (microbiologia, glúten, cloro e outros).
- Avisos para Manutenção ou Higienização quando for preciso intervir.

*O que podemos escolher para ver nos dashboards*
- Incidências.

**Higienização — equipa interna**
- Catálogo de produtos (com fichas técnicas e de segurança).
- Plano por dias e zonas, registo de execução com nome e assinatura.
- Fotos “antes e depois” quando fizer sentido.

*O que podemos escolher para ver nos dashboards*
- Cumprimento do plano por semana e por área, faltas nas limpezas, incidencias que vem do modulo da qualidade.

**Higienização — equipa externa**
- Igual à interna, mas separado: planos, execuções e superfícies diferentes, confirmações de presença.

**Controlo de rotulagem com inteligência artificial**
- Fotografia da etiqueta → o sistema lê os textos → compara com a nossa base de dados.
- Itens críticos (lote, datas, lista de ingredientes, alergénios): **aprovado**, **rejeitado** ou **colocada para revisão humana**.
- Pequenos avisos para diferenças menos importantes (ex.: pontuação errada, ordem dos ingredientes errada(o que também pode ser crítico) ).

*O que podemos escolher para ver nos dashboards*
- Percentagem de etiquetas aprovadas à primeira, erros por tipo, com historico e detalhes da maquina, produto etc.

---

### 3.4. Manutenção

- Registo de preventivas (calendário), corretivas, externas etc(como já temos no SARA(manuela)).
- Peças de reposição com controlo de stock separado do armazém com scan de QR code.
- Documentos de apoio e responsáveis por secção.

*O que podemos escolher para ver nos dashboards*
- Falhas por equipamento, tempo médio de reparação, calendário ou cumprimento do plano de preventivas.

*Sugestões*
- Quando Produção ou Qualidade registam uma avaria, abrir uma folha de obra automaticamente, mas apenas o responsável da secção teria a possibilidade de registar uma avaria.
- Podemos criar outro canal alternativo, mais para incidências, onde todos podem dizer, "a máquina parou" e geralmente o responsável da máquina ou secção decidir se é uma coisa que se pode fazer na hora ou registar uma avaria para a manutenção.
- Criar um aviso para o departamento, das incidências e falhas dos equipamentos.
- Criar responsáveis por máquina também. Na falta do principal responsável e eventualmente um substituto, o responsável da secção seria o responsável da máquina automaticamente.

---

### 3.5. Pessoas e Comunicação

**Colaboradores e contas**
- Cada pessoa tem uma conta e podemos usar/associar cartões ou nfc nos locais ou no proprio dispositivo para registar presenças ou para desbloquear certas zonas/maquinas.
- No ecrã inicial, a pessoa vê só os módulos do seu departamento. Dentro de cada módulo, o papel detalhado é definido pelo responsável.

**Dashboards com informação ao vivo**
- Ecrã da Administração: visão do dia (quantidades produzidas, paragens e motivos, lotes bloqueados, encomendas prontas, leituras importantes, incidentes).
- Televisores na fábrica, refeitorio, zonas sociais: mensagens positivas, ranking de equipas(quantidade de registos, quantidade de falhas), informações úteis e avisos .
- Modo para visitas: ecrã bonito, sem nomes de pessoas, com animação na abertura e destaque do que correu bem, também com posibilidade de alterar dados por trás.

**Mensagens e agradecimentos no feed ou nas dashboards**
- Anúncios da direção (com possibilidade de pedir confirmação de leitura, no caso das auditorias importantes ex: amanhã auditoria X, precisamos ter em atenção 1. 2. e 3. e para continuar confirma que leu e que vai cumprir cum as regras).
- Podemos estabelhecer marcas importantes e com agradecimentos automáticos quando são atingidos.
- Pedidos formais de tarefas para os departamentos certos ou com possibilidade de alguem escolher uma tarefa(ex: precisamos de 2 pessoas para fazer X).
- Pedidos formais dos responsáveis de secção(ex: estamos sem 2 funcionários esperamos nomeação de 2 substitutos e aí alguém associa as pessoas para esse departamento e os responsáveis das secções dos tais funcionarios e os proprios funcionarios podem receber notificação para mudar de secção)

**Sugestões e reclamações (anónimas ou públicas)**
- Canal onde qualquer um pode deixar uma ideia ou apontar um problema.
- A direção pode até responder mensagens directas ou públicas mas.

---

## 4) Ecrãs com informação ao vivo (O que podemos escolher para ver nos dashboards)

- Quantidades produzidas hoje, com comparação simples com a média da semana.
- Paragens por linha e motivos mais comuns.
- Leituras de controlo importantes (por exemplo, temperaturas e verificações de segurança).
- Encomendas prontas, cargas em preparação e o que já saiu.
- Incidentes e ocorrências ainda por resolver.
- Consumos de vários tipos(energia, agua, intervenções técnicos externos etc.)

---

## 5) Quando a internet falha (vai acontecer até o servidor falhar)

- Sem internet a aplicação continua a funcionar na rede interna quando há servidor ou os registos ficam guardados nos dispositivos e seguem quando houver ligação com o servidor.
- Processos que dependem do exterior (por exemplo, envio de e‑mail automático, n8n e encomendas h3) geralmente tem retry a cada 30 minutos.
- Mas se o automatismo falhar mesmo de 30 em 30 minutos e não há tempo para esperar por eles, podemos implementar uma forma de inserir as encomendas, anexando os pdf's ou edi's ou até inserindo 1 a 1.
- Podemos ter um dossier em algum lugar com os modelos em papel e imprimir se a falha for grave e ficar sem app (ter em papel um formulario mais parecido com o digital para ser fácil de preencher por todos)

---

## 6) O que ganhamos como empresa

- Menos papel, menos duplicações e menos erros.
- Velocidade em alguns departamentos (como no controlo de rotulagem ou criação da folha de produção se tentarmos automatizar ao máximo as encomendas que vem por email, edi, ou mensagens, ou até pot voz se utilizarmos o workflow já criado em n8n e o modelo openAI whisper para transcrever o audio)
- IFS vai adorar
- Decisão mais rápida: todos veem os mesmos números e a mesma realidade do dia.
- Cultura positiva: informação clara, reconhecimento, e voz para quem está no terreno.
- Os funcionários sentem que fazem parte da empresa.

---

## 7) Outras sugestões

- Implementar um sistema de criação de novos produtos onde cada departamento preenche o que for da responsabilidade deles e apenas quando todos sabem do que se trata e temos as informações completas, aprovadas por administração e dep. de qualidade, podemos avançar com a produção. Dessa forma, com a informação de cada um, conseguimos gerar uma ficha tecnica em pdf, completa, antes de começar a produzir e sem falar que não há dúvidas pelo caminho do tipo "pico no 3? qual o molde? tem artigo? qual a etiqueta? em que caixa vai? quantos dias de validade?" e muitas muitas outras perguntas que algumas pessoas escutam quase todos os dias sem necessidade.
- Criar outros módulos que eu agora não consegui imaginar, talvez um departamento de compras ou RH.. claro precisamos de uma coisa dessa com o RH, marcar férias, ausencias, colocar documentos(se não for usar o idonic). Teriamos uma limitação no idonic, um só pc no refeitorio para as pessoas ficar marcando e desmarcando ferias ou ausencias não vai dar muito certo, cada um no seu celular consegue fazer isso com mais tranquilidade e até em casa.


**É um projeto extremamente complexo, várias vezes mais dificil de criar do que o SARA mas não impossível. Quando criei o SARA nem imaginava que ia chegar ao tamanho que o SARA tem hoje. Sempre pensava assim, "ah eu sei", e quando ia tentar descobria que não sabia nada ou não era possivel fazer em appsheet, mas dei um jeito. Por mais que foi criado com appsheet, uma feramenta chamada de "Low-Code", a complexidade do SARA é bem alta. Eles dão algumas opções e tu tens que trabalhar com aquilo e um pouco de magia.**

**Fazer um app 100% nosso não tem limites como no appsheet mas é muito mais dificil de aprender. Mas eu estou confiante que vai dar certo porque o modulo de expedição h3 e da folha de produção já estão funcionais, tem coisas novas, modernas e que eu nem pensava ser capaz.**
