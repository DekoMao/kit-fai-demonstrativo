# Kit demonstrativo de preparação e registro de FAI

Ferramenta educacional gratuita de **Wanderley Uchôa**, voltada à organização de referências e evidências de inspeção do primeiro artigo.

## Uso

Abra `index.html` no navegador ou utilize a página publicada pelo GitHub Pages. Use o exemplo simulado, comece em branco e salve o registro em JSON. O CSV exporta apenas as características. O botão de download fornece o pacote para uso offline.

## Quatro blocos

1. Configuração e escopo: produto, desenho/revisão, serial/lote e comparação de referências.
2. Características: requisito, limites, unidade, resultado, instrumento e referência de evidência.
3. Pendências e decisão: impacto, verificações, disposição e responsável autorizado.
4. Mudanças: alteração, impacto e vínculo documental.

## Exemplo simulado

| Característica | Faixa inclusiva | Resultado | Comparação |
|---|---|---|---|
| Comprimento do suporte | 99,8–100,2 mm | 100,1 mm | Dentro da faixa |
| Largura do suporte | 59,8–60,2 mm | 60,3 mm | Fora da faixa |
| Tensão de saída da montagem | 4,9–5,1 V | Ausente | Pendente |

O ensaio elétrico pertence à montagem e à instrução de teste, não ao desenho do suporte. Os dados e referências são simulados e independentes de qualquer organização.

## Limites

Modelo independente; não é formulário oficial AS9102/EN9102 e não declara conformidade normativa. A comparação numérica não considera incerteza de medição, regra de decisão ou adequação do instrumento. Não libera produto. Os campos de nome e data não são assinaturas autenticadas. O histórico é editável; as referências de evidência não anexam nem verificam arquivos. Adapte ao contrato e ao procedimento aplicável.

## Dados

Sem backend, analytics ou dependências externas no aplicativo. Os campos são processados no navegador; o preenchimento não é enviado pela ferramenta. O provedor de hospedagem pode registrar dados técnicos de acesso. Não há salvamento automático entre sessões. Preserve o JSON em local autorizado.

## Testes

Execute `node tests/validar.cjs`. Testes de lógica cobrem limites inclusivos, entradas inválidas, campos vazios, vírgula decimal, zeros em identificadores, importação validada, JSON/CSV e IDs duplicados. Não equivalem a certificação nem substituem avaliação do processo.

## Publicação

Site estático, sem build. No GitHub Pages, publicar a branch `main`, pasta `/ (root)`. Não contém arquivo corporativo de terceiros nem dados de inspeção reais.

## Referências de pesquisa

- https://www.guthcad.com/as9102-FAI-Portuguese.html
- https://fileit.com/form-templates/first-article-inspection

Versão demonstrativa 1.1 • 23/11/2026.
