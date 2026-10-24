# Plano: de técnico químico a consultor PJ em dados de processo (celulose e papel)

Perfil: técnico em química, 15 anos em papel e celulose, estudante de Engenharia de Software, Python básico.
Ritmo: 1 h/dia (~7 h/semana). Sem acesso a dados reais, então usamos bases públicas.
Posicionamento: **dados de processo e qualidade para a indústria de celulose e papel**
(soft sensors, previsão de falhas, quimiometria). RDKit/QSAR entra como módulo curto.

## Fases (a ~7 h/semana)

| Fase | Semanas | Foco | Entrega comprovável |
|---|---|---|---|
| 0 | 1 | Ambiente: VS Code, Git, Miniforge, Jupyter, repositório GitHub | "Hello data" versionado |
| 1 | 2–6 | Python de verdade, pandas, estatística descritiva, gráficos, Git | EDA completa da base Kamyr digester |
| 2 | 7–14 | **Projeto 1: soft sensor de número kappa** (regressão, validação temporal, PLS, métricas, limitações) | Repositório com README, testes e relatório |
| 3 | 15–22 | **Projeto 2: previsão de quebra de papel** (séries temporais, eventos raros, desbalanceamento, curva PR) | Repositório + relatório de validação |
| 4 | 23–30 | SQL/PostgreSQL, quimiometria (PCA/PLS em espectros NIR), KNIME básico | Banco consultável + notebook de quimiometria |
| 5 | 31–38 | RDKit (ESOL) como módulo, engenharia (módulos, pytest, CI, Docker), dashboard | Projeto 3 + dashboard |
| 6 | 39+ | Mercado: LinkedIn, vagas, freelas, proposta de consultoria PJ | Primeiros contatos e propostas |

Marcos de mercado (estimativas, não promessas):
- Mês 4–5: já dá para se candidatar a vagas de analista de dados industrial (sua experiência pesa muito).
- Mês 9–15: primeira posição ou freela na área.
- Ano 2–3: consultoria PJ sustentável, dependente de entregas reais e rede de contatos.

## Bases públicas confiáveis

- **Kamyr digester** (previsão de número kappa, soft sensor, 301 observações, 22 variáveis, CC BY-SA 4.0):
  https://datahub.io/@olayway/datapackage-factory-openMV/kamyr-digester
  Versão estendida e exercício de referência: https://learnche.org/latent/Assignment_4
- **Quebras de papel** (61 sensores, série temporal, eventos raros, Bo Peng, Figshare, fev/2025):
  https://figshare.com/articles/dataset/sensors-data-processminer-rare-event-mts_xlsx/28376027
  (Conferir licença na página antes de publicar qualquer coisa derivada.)
- Complementares: Tennessee Eastman, Debutanizer/SRU (soft sensors), Tecator (NIR), ESOL/Lipophilicity (MoleculeNet).
- Sintético: simulação de cozimento kraft com seu conhecimento de processo, sempre rotulada como sintética.

Regra: antes de usar qualquer base, registrar fonte, licença, unidades, variáveis e limitações.

## Padrão de entrega de cada projeto

1. Problema de negócio em linguagem de fábrica (custo, qualidade, parada).
2. Dados: fonte, licença, qualidade, tratamento de ausentes e outliers.
3. Baseline simples antes de modelo complexo.
4. Validação correta (temporal quando houver tempo; sem vazamento de dados).
5. Erros inspecionados e limites de uso do modelo.
6. README, testes, dependências, instruções de execução.
7. Explicação em 5 minutos: problema, dados, método, resultado, limitações.

## Regras de honestidade

- Não declarar experiência em ferramenta que não foi praticada.
- Previsão não é medição.
- Nada de dado confidencial de empresa sem autorização formal.
- Projeto com dado público é portfólio, não experiência profissional; dizer isso com clareza.
