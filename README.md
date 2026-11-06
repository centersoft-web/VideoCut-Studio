# 🎬 StudioCut

Editor de vídeos curtos executado diretamente no navegador, desenvolvido em **HTML, CSS e JavaScript puro**.

O StudioCut oferece uma interface visual para montar projetos com vários clipes, aplicar cortes, filtros, textos, stickers, trilha sonora, transições e áreas de privacidade. O processamento acontece localmente no navegador, sem necessidade de servidor ou instalação.

## ✨ Principais recursos

### Projetos

- Criação de múltiplos projetos
- Biblioteca de projetos salvos no navegador
- Abrir, renomear, duplicar e excluir projetos
- Comando **Salvar projeto como…**
- Edição não destrutiva: os arquivos originais importados são preservados
- Indicador de alterações não salvas
- Histórico de desfazer e refazer

### Clipes e edição

- Importação de um ou vários vídeos
- Corte individual de início e fim
- Reordenação dos clipes por arrastar e soltar
- Controle individual de velocidade, de `0,25×` a `2×`
- Formatos de projeto:
  - `16:9` horizontal
  - `9:16` vertical
  - `1:1` quadrado

### Transições

- Dissolver
- Fade pelo preto
- Deslizar
- Zoom
- Corte direto
- Controle de duração
- Pré-visualização da transição

### Trilha sonora

- Importação de arquivos de áudio
- Reprodução sincronizada com a prévia
- Controle de volume da trilha
- Controle independente do áudio original
- Fade de entrada
- Fade de saída
- Repetição automática da música quando necessário

### Textos e stickers

- Vários textos e stickers no mesmo projeto
- Posicionamento por arrastar
- Controle de tamanho e cor
- Definição do momento em que cada elemento aparece e desaparece
- Exclusão individual de camadas

### Privacidade

- Várias áreas pixeladas ou desfocadas
- Posicionamento por arrastar
- Redimensionamento pelo mouse ou toque
- Ajustes precisos de largura e altura
- Controle do tamanho do quadriculado
- Controle da intensidade do desfoque
- Controles de seleção ocultos quando a área não está selecionada

### Filtros

- Normal
- Cinema
- Preto e branco
- Quente
- Frio
- Vintage
- Ajustes manuais de brilho, contraste e saturação

### Exportação

- Exportação para MP4 quando suportado pelo navegador
- Alternativa automática em WebM
- Composição de cortes, filtros, textos, stickers, máscaras e trilha
- Nome exclusivo para cada arquivo exportado
- Indicador de progresso
- Estimativa de tempo
- Tratamento de erros e limpeza de recursos ao concluir

## 🚀 Como usar

1. Baixe o arquivo `index.html`.
2. Abra o arquivo em um navegador moderno.
3. Clique em **Escolher clipes** e selecione um ou mais vídeos.
4. Ajuste os cortes, a ordem e a velocidade dos clipes.
5. Adicione transições, trilha sonora, textos, stickers, filtros ou áreas de privacidade.
6. Clique em **Salvar projeto como…** para guardar o projeto no navegador.
7. Escolha o formato desejado e clique em **Exportar vídeo**.

> O editor não altera os arquivos originais. O projeto salvo e o vídeo exportado são novas cópias.

## 💾 Salvamento dos projetos

Os projetos são armazenados localmente no navegador por meio do **IndexedDB**.

- O salvamento não é automático.
- Use **Salvar projeto como…** sempre que quiser gravar o estado atual.
- Alterações posteriores ficam marcadas como não salvas.
- Os projetos ficam disponíveis apenas no mesmo navegador e dispositivo.
- Limpar os dados do navegador pode remover os projetos armazenados.
- Vídeos e áudios grandes podem consumir uma quantidade significativa do armazenamento local.

## 📁 Estrutura

```text
studiocut/
├── index.html
└── README.md
```

Todo o aplicativo está contido em um único arquivo HTML:

- Estrutura da interface em HTML
- Estilos responsivos em CSS
- Lógica do editor em JavaScript
- Processamento visual com Canvas API
- Mixagem de áudio com Web Audio API
- Exportação com MediaRecorder API
- Armazenamento de projetos com IndexedDB

## 🌐 Compatibilidade

Recomenda-se usar uma versão atual de:

- Microsoft Edge
- Google Chrome
- Mozilla Firefox
- Safari

A disponibilidade de MP4 depende dos codecs oferecidos pelo navegador. Quando MP4 não estiver disponível, use WebM ou mantenha a opção automática.

## ⚠️ Limitações conhecidas

- A exportação é realizada em tempo real e pode levar aproximadamente a duração do projeto.
- O desempenho depende do tamanho, resolução e quantidade de clipes.
- Arquivos muito grandes podem ultrapassar o limite de armazenamento do navegador.
- A compatibilidade de áudio e vídeo varia conforme os formatos aceitos pelo navegador.
- O editor funciona inteiramente no navegador e não substitui um editor profissional para projetos longos ou muito complexos.

## 🔐 Privacidade

Os arquivos são processados localmente no navegador. O StudioCut não possui servidor próprio, login, telemetria ou integração de envio de arquivos.

Mesmo assim, use apenas mídias que você tenha autorização para editar e compartilhar.

## 🧰 Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript
- Canvas API
- Web Audio API
- MediaRecorder API
- IndexedDB
- Blob e Object URLs
- Drag and Drop API
- Pointer Events

## 🛠️ Desenvolvimento

O projeto não requer instalação de pacotes, compilação ou servidor de desenvolvimento.

Para editar:

1. Abra `index.html` em um editor de código.
2. Faça as alterações desejadas.
3. Salve o arquivo.
4. Atualize a página no navegador.

Para testar alterações de armazenamento de maneira isolada, use um perfil separado do navegador ou limpe somente os dados do site após exportar os projetos importantes.

## 🗺️ Possíveis melhorias futuras

- Importar e exportar projetos como arquivo JSON
- Miniaturas dos projetos na biblioteca
- Formas adicionais para máscaras de privacidade
- Animações de entrada e saída para textos
- Ondas de áudio na linha do tempo
- Atalhos de teclado configuráveis
- Controle de qualidade e resolução da exportação
- Legendas automáticas ou importação de arquivos de legenda

### Instalação no computador

### No Google Chrome ou Microsoft Edge:

  1. Abra o endereço publicado do projeto.
  2. Aguarde o carregamento completo da página.
  3. Clique no ícone de instalação exibido na barra de endereço ou abra o menu do navegador.
  4. Selecione Instalar aplicativo ou Instalar este site como aplicativo.
  5. Confirme a instalação.

Depois disso, o aplicativo poderá ser aberto pelo menu Iniciar, pela área de trabalho ou pelo gerenciador de aplicativos do sistema.

### Instalação no celular ou tablet

### Em navegadores compatíveis:

1. Abra o endereço do projeto.
2. Acesse o menu do navegador.
3. Selecione Instalar aplicativo ou Adicionar à tela inicial.
4. Confirme o nome e a instalação.

O ícone será adicionado à tela inicial do dispositivo.

**Observações**

A disponibilidade e o nome da opção de instalação podem variar conforme o navegador e o sistema operacional.
Abrir somente o arquivo index.html pelo computador não garante a instalação como PWA.
O projeto deve ser publicado em HTTPS para utilizar os recursos completos de instalação e service worker.
O funcionamento offline depende da configuração do service-worker.js e dos arquivos adicionados ao cache.
Atualizações no projeto podem exigir a atualização da versão do cache do service worker.

## Licença

Nenhuma licença específica foi definida no arquivo fornecido. Antes de distribuir ou publicar o projeto, inclua uma licença compatível com a finalidade pretendida e verifique as licenças das bibliotecas externas utilizadas.


## Aviso

> Este projeto é uma demonstração educacional desenvolvida para estudos de HTML, CSS e JavaScript. A empresa mencionada é fictícia e qualquer semelhança com empresas reais é mera coincidência.

---

Desenvolvido como um editor de vídeos curtos, local e independente, com foco em simplicidade, privacidade e edição não destrutiva.
