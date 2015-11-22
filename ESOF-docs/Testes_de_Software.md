#Testes de Software

**Introdução**

O Kodi, como já foi dito nos trabalhos anteriores, é desenvolvido numa estrutura modular, módulos estes que são independentes uns dos outros, permitindo compilar o software mesmo que um módulo ou biblioteca não essencial esteja desativado ou tiver sido removido. Este tipo de desenvolvimento torna-se também bastante útil no caso dos testes por se poder isolar o que se pretende testar e por cada componente a ser testado ter uma responsabilidade bem definida. Para além dos próprios testes criados, o Kodi possui também uma ferramenta chamada Jenkins. Esta ferramenta é utilizada quando algum utilizador pretende fazer um *pull request* no github e a sua função é fazer *build* do projeto, caso a *build* seja bem sucedida, ou seja, se não houver erros, o projeto passa a ser *safe to merge*, podendo posteriormente ser integrado no projeto *master* do Kodi. O Kodi tem ainda um modo de debugging em runtime que grava e imprime o estado do software.

Os módulos de teste do Kodi utilizam a unit testing library gtest.

**1.Degree of Testability of the software program**

* Controllability

Os componentes são testados por atribuição de diversos valores de entrada. Ou seja, a classe correspondente ao componente é criada com certos valores e, utilizando a api do gtest, o resultado é comparado a certos valores esperados. Como os componentes não são muito complexos este método não é bastante eficaz.

* Observability

O resultado dos testes vem no estado true ou false, sendo que no segundo é imprimido também o valor esperado e o obtido. Este método embora eficaz não nos permite identificar erros intermédio directamente.


* Isolateability

Como já anteriormente referido, cada componente do Kodi é desenvolvida de forma independente, podendo esta funcionar independentemente do resto do programa. Assim sendo é possivel testar isoladamente cada uma destas.


* Separation of concerns

Cada componente testada tem uma responsabilidade bem definida. O software está estruturado perante esse premissa e podemos identificar isso pela simplicidade de cada um dos componentes.


* Understandability

Todas as componentes do Kodi estão extensivamente comentadas, apenas com uma simples consulta ao ficheiro .h correspondente conseguimos compreender o objectivo e forma de funcionamento da componente.


* Heterogeneity

O software usa apenas uma tecnologia para testar cada componente(gtest). Usa ainda jenkins para garantir a integridade do software no seu todo. É possivel ainda criar um log em runtime do software que grava e imprime todos os eventos estranhos ao software.


**2.Test Statistics**

* Localização dos testes:
kodi(https://github.com/dua123/xbmc/tree/master/xbmc/test)
addons(https://github.com/dua123/xbmc/tree/master/xbmc/addons/test)
filesystem(https://github.com/dua123/xbmc/tree/master/xbmc/filesystem/test)
musictag(https://github.com/dua123/xbmc/tree/master/xbmc/music/tags/test)
network(https://github.com/dua123/xbmc/tree/master/xbmc/network/test)
threads(https://github.com/dua123/xbmc/tree/master/xbmc/threads/test)
utils(https://github.com/dua123/xbmc/tree/master/xbmc/utils/test)
video(https://github.com/dua123/xbmc/tree/master/xbmc/video/test)

* Número de teste encontrados: 71 testes.
Embora o número de testes seja relativamente alto, o número de componentes presentes no software também é e nem todas estão a ser testadas. A filosofia do Kodi passa mais por, compilar, correr o programa e ver se funciona como estava previsto. Esta abordagem não é a melhor em programas tão complexos e que envolvam um grande número de pessoas, no entanto, a boa estruturação de código e desenvolvimento modular torna isto possível.
