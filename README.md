WebSIG - Sistema de Informacao Geografica Interativo

Este e um projeto de WebSIG (Sistema de Informacao Geografica para a Web) interativo, desenvolvido em Python utilizando a biblioteca Folium. O mapa foi projetado para carregar de forma rapida, eficiente e automatizada, integrado diretamente com o GitHub Pages para visualizacao publica.

## Acesse o Mapa Online

O mapa esta publicado e pode ser acessado atraves do link :https://engcarto-paulo.github.io/WebSIg-Desenvolvimento/



 Funcionalidades do Projeto

Enquadramento Automatico: O mapa abre focado exatamente nas coordenadas limites (bounds) da area de estudo, sem necessidade de busca manual.
  Multiplas Camadas de Fundo (Basemaps): Seletor interativo para alternar entre Satelite Google, Satelite Esri World Imagery, OpenStreetMap e Mapas Tematicos Claro e Escuro (CartoDB).
 Ortomosaico Otimizado: Processamento e compressao de imagem raster (TIF) com remocao de bordas pretas ou brancas e transparencia (RGBA), otimizado para carregamento rapido na web.
 Camadas Vetoriais (GeoJSON): Includes Lotes (delimitacao em amarelo pastel fosco), Edificacoes (poligonos em vermelho terracota com transparencia), Eixo de Rua (linhas em cinza escuro charcoal) e Area Verde (poligonos em verde floresta).
 Pop-ups Dinamicos: Consulta de atributos cadastrais diretamente ao clicar em qualquer feicao do mapa.
 Legenda Suspensa: Legenda compacta integrada ao layout para facil interpretacao das cores das camadas.
 Ferramentas de Medicao e Desenho: Painel completo para medir distancias (metros e quilometros), areas (metros quadrados e hectares) e desenhar geometrias com opcao de exportacao automatica para GeoJSON.

---
 Tecnologias Utilizadas

O processamento espacial e a geracao do ambiente SIG foram feitos utilizando as seguintes bibliotecas em ambiente Python dentro do Google Colab:

* Geopandas: Para manipulacao e reprojecao de dados vetoriais (GeoJSON).
* Rasterio: Para leitura, reprojecao (UTM para WGS84) e downsampling (reducao de amostragem) do ortomosaico.
* Folium e Branca: Para a renderizacao do mapa interativo em HTML, injecao de scripts Leaflet.js e criacao de elementos customizados como a legenda.
* Pillow (PIL) e NumPy: Para tratamento de matrizes de imagem e compressao avancada do arquivo final.

---

## Estrutura de Arquivos Gerados

* index.html: Arquivo principal do site que contem toda a estrutura do WebSIG, scripts e dados embutidos (renderizado via GitHub Pages).
* ortomosaico_transparente.png: Imagem gerada com compressao maxima utilizada como sobreposicao no mapa.

---

## Autor

Desenvolvido por Paulo H Soares- Engenharia  Cartografia e de Agrimensura-UFPR.
