# 423.-Padrao-MVC
Aula teória

{
 M - Model
   É a camada que se liga ao banco de dados, caso seja solicitado demonstração de informações,
   ou acessar dados (ex visualizar uma tela sem renderisar).
 V - View
 C - Controler
     Controler é um intermediador entre Model e View, é uma espécie de Gerenciador
     é uma especie de Secretária que se denomina FrameWork MVC, um arquivo que contem as rotas
    para coordenar o fluxo de dados como uma recepção que distribui para cada morador.
  
  Fluxo.
  Um Browser gerando uma requisicao a partir de uma URL, tal requisição vai bater em seu 
  webserver (ex. Toncat. Enjoynext, Apache depende da tecnologia que voce usa etc...), ele direciona 
  para um aplicação e seu FrameWork MVC vai destinar para onde vai a requisição.
  Essa é a primeira camada onde a requisição chega no Controler.
  
  Exemplo de Fluxo 1;
      Browser - requisicao de tela simples com menu;
            Controler - encaminha para;
                View - processa e devolve para o Browser;
                
  Exemplo de fluxo 2;
        Browser - requisicao de lista de clientes;
            Controler - solicita a lista para;
                Model - busca a informação e devolve;
                    Controler - solicita outra lista com clientes excluidos por ex;
                          Model - busca a informação novamente e devolve;
                              Controler com sua necessidade atendida encaminha para;
                                  View - processa e devolve para o Browser;
}
