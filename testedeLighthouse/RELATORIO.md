# Relatório de atividade prática: analisando e melhorando a performance do site com Lighthouse

**Nome:** ____________________________  **Turma:** __________

## 1. Objetivo
Avaliar a performance, a acessibilidade, as melhores práticas e o SEO de um site institucional e realizar mudanças que possam melhorar a experiência dos usuários.

## 2. Site e configuração do teste
Foi preparado um **site demonstrativo fictício**, chamado EcoStart, com duas versões: `index_inicial.html` (antes) e `index.html` (depois). O Lighthouse deve ser executado no Google Chrome, com as categorias **Performance, Acessibilidade, Melhores Práticas e SEO** selecionadas. **Dispositivo usado:** [preencher: Mobile ou Desktop].

**Importante:** as auditorias reais ainda não foram executadas. Não foram inventadas pontuações. Abra cada versão em ambiente web e salve os relatórios gerados pelo Lighthouse para completar esta parte.

## 3. Resultados do Lighthouse

| Categoria | Versão inicial | Versão final |
|---|---:|---:|
| Performance | [pontuação] | [pontuação] |
| Acessibilidade | [pontuação] | [pontuação] |
| Melhores Práticas | [pontuação] | [pontuação] |
| SEO | [pontuação] | [pontuação] |

**Principais alertas do relatório inicial:** [registrar alertas apresentados pelo Lighthouse].

**Principais alertas do relatório final:** [registrar alertas apresentados pelo Lighthouse].

## 4. Melhorias implementadas
1. **Imagens otimizadas:** foram utilizadas ilustrações SVG leves e escaláveis, evitando imagens fotográficas pesadas; o projeto inclui dimensões explícitas nas imagens.
2. **Minificação de recursos:** o CSS e o JavaScript foram colocados em arquivos compactos (`style.min.css` e `script.min.js`), com menos espaços e quebras desnecessárias.
3. **Carregamento atrasado:** foi aplicado `loading="lazy"` à imagem da seção de serviços, que aparece abaixo do conteúdo inicial.
4. **SEO:** foram incluídos título descritivo, `meta description`, `meta robots`, idioma do documento e `meta viewport`.
5. **Acessibilidade:** imagens receberam textos alternativos; o site usa regiões semânticas; foi criado um link para pular ao conteúdo; os links exibem foco visível para navegação por teclado.
6. **Execução de scripts:** o JavaScript foi carregado com `defer` para não bloquear o processamento inicial do HTML.

## 5. Análise das mudanças e impactos
As mudanças foram planejadas para tornar o site mais leve, acessível e fácil de encontrar em mecanismos de busca. O uso de SVG evita arquivos de imagem desnecessariamente grandes; o carregamento atrasado adia recursos que não são necessários imediatamente; e a minificação reduz o tamanho dos arquivos de código. As descrições das imagens, a navegação por teclado e as tags semânticas contribuem para a acessibilidade. As meta tags e o título descritivo ajudam os mecanismos de busca a compreender o conteúdo. **A confirmação de ganhos nas pontuações depende da comparação dos dois relatórios reais do Lighthouse.**

## 6. Conclusão
A atividade demonstrou que otimizar imagens, compactar recursos, aplicar carregamento atrasado e melhorar acessibilidade e SEO são medidas importantes na construção de sites. Após a execução do Lighthouse nas duas versões, será possível verificar quais melhorias aumentaram as pontuações e quais problemas ainda precisam de ajustes.

## 7. Como finalizar a entrega
1. Sirva a pasta com um servidor local (por exemplo, extensão Live Server do VS Code), abra `index_inicial.html` no Chrome e gere o primeiro relatório na aba **Lighthouse** do DevTools.
2. Abra `index.html` no mesmo ambiente e com o **mesmo dispositivo e categorias**; gere o segundo relatório.
3. Exporte/salve ambos os relatórios Lighthouse, preencha a tabela acima e anexe os dois arquivos ao entregar.
4. Entregue também `index.html`, `style.min.css`, `script.min.js` e a pasta `imagens/`.

> Os arquivos `index_inicial.html` e `index.html` são uma demonstração criada para a atividade, não uma auditoria de um site real da startup.
