Introdução

O nosso projeto é o Kodi, uma multiplataforma de entretenimento, desenvolvida pela fundação xbmc, fundação sem fins lucrativos, com a particiação de *Developers* de todo o mundo para o desenvolvimento e melhoramento das diferentes características do software, essencialmente no github.
O Kodi deixa-nos ver filmes,ouvir música e ver fotos, de modo *user friendly* , tendo o utilizador a possibilidade de interagir com toda a sua multimédia.
Este permite  ainda a utilização de *add-ons*, expandindo assim o leque de funcionalidades possíveis, entre as quais a visualização de conteudos em *stream* ou *download* de fontes exteriores(clouds,spotify,youtube,etc...).

Software Process

A equipa de desenvolvimento do Kodi utiliza como base um processo de desenvolvimento de software que segue um modelo iterativo incremental, tendo em conta que o software está estruturado de uma forma modular rigorosa.

Tendo o Kodi um design modular, é-lhe permitido crescer e evoluir de uma forma eficiente uma vez que se pode inserir novos módulos ao software, sem termos o problema de o software deixar de funcionar o que facilita bastante a gestão do software.

Qualquer módulo pode ser alterado sem afetar diretamente o funcionamento dos outros. Estes módulos são separados em grupos funcionais que são independentes uns dos outros, entre eles temos, *skins*(trata dos diferentes visuais do software, *interfaces*(módulo onde são criadas novas funcionalides), a gestão de conteúdo, o núcleo do software(onde se torna possível a reprodução de ficheiros de video e áudio) e por fim a partilha de ficheiros(módulo desenvolvido para ser possível o *download* e *stream* e partilha de ficheiros).

Kodi, pela análise feita, usa um modelo de desenvolvimento iterativo incremental em que combina as vantagens do modelo queda d'água com o modelo de prototipação, neste sistema existe um desenvolvimento de forma incremental, até que exista um produto estável para lançamento.
Uma vantagem desta abordagem é a facilidade de testar o sistema, visto que este é testado em todas as iterações, diminuindo riscos a falhas no projecto global, fazendo com que o produto final seja um produto estável para mercado. Mesmo builds estáveis estão sujeitas a teste e possíveis modificações. Em cada nova iteração, especialmente as que seguem *builds* estáveis, a contribuição de todas as pessoas envolvidas no projecto é analisada, decidindo-se assim as próximas alterações a serem feitas no software, a implementar numa nova *build*. E o ciclo continua.

Esta abordagem permite-nos aproveitar ao máximo a contribuição de todos os envolvidos enquanto se mantem a integridade do software.


Requerimentos

- Primeiro que tudo ser orientado para ecrãs grandes(28 ou mais polegadas) para uma experiência de "sala";
  - Menus grandes, tipo de letra e botões próprios para serem navegados a partir de um comando;
- Ser focado em torno das funcionalidades principais que são ouvir música, ver filmes, gravar programas televisivos e ver fotografias;
  - O Kodi pode ser capaz de nos trazer outras funcionalidades mas estas nunca podem tirar o foco das principais;
- Ter uma instalação e utilização fáceis e intuitivas para não intimidar pessoas com menores conhecimentos técnicos;
- Ser capaz de reproduzir ficheiros de vídeo e áudio no formato DivX, XviD, etc, sem ser necessário novas instalações;
- Permitir a organização de ficheiros de áudio e vídeo de uma maneira fácil e amiga do utilizador;
- Usar padrões e ser consistente (a secção de música não pode ter controlos completamente diferentes da de vídeo);
- Realizar tarefas no menor número de cliques possível;
- Ser orientado a uma audiência internacional podendo suportar diferentes línguas, fusos-horários e outras diferenças entre regiões;
- Requerer pouca ou nenhuma configuração *non-GUI* (e toda esta deve ser apenas incluída num ficheiro: advancedsettings.xml);
- Ser esteticamente atrativo.
