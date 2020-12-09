função  preencher ( linkName )  {
    documento . getElementById ( "menu" ) . innerHTML = '' ;

    var  link  =  "https://restaurant12032020.herokuapp.com/"  +  linkName ;

    buscar ( link )
        . então ( resposta  =>  resposta . json ( ) )
        . então ( json  =>  {
            para  ( seja  i  =  0 ;  i  <  json . comprimento ;  i ++ )  {
                 cartão  var =  documento . createElement ( "div" ) ;
                cartão . className  =  "cartão" ;

                var  content  =  `<img class =" card-img-top "src =" item-img "alt =" Imagem do cartão ">
                    <div class = "card-body">
                    <h4 class = "card-title"> nome do item </h4>
                    <h6 class = "card-subtitle mb-2 text-danger"> oferta de item </h6>
                    <p class = "card-text"> item-des </p>
                    <div class = "buy d-flex justify-content-between align-items-center" id = "price">
                    <div class = "price text-success"> <h5 class = "mt-4"> $ item-price </h5> </div>
                    </div>
                    </div> ` ;
                
                    conteúdo  =  conteúdo . substituir ( "nome do item" ,  json [ i ] . nome ) ;
                    conteúdo  =  conteúdo . substituir ( "item-img" ,  json [ i ] . imagem ) ;
                    conteúdo  =  conteúdo . substituir ( "item-des" ,  json [ i ] . descrição ) ;
                    conteúdo  =  conteúdo . substituir ( "item-oferta" ,  json [ i ] . oferta ) ;
                    conteúdo  =  conteúdo . substituir ( "ponto-preço" ,  json [ i ] . preços ) ;
                                
                    cartão . innerHTML  =  content ;

                    documento . getElementById ( "menu" ) . appendChild ( cartão ) ;
                
            }
        } )
}
