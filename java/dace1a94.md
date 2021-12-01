# Static blocks

A static block will run only once. Generally used for configure something, only one time, without the need of create a method.

>
Um exemplo, você tem um mapa estático e quer deixar seus valores inicializados. Você até pode fazer new no map sem o bloco, mas não consegue chamar o método “put” lá. Então vc usa um bloco estático.

´´´
public class Router {
private static final Map<String, String> routes = new HashMap<String, String>();
 static {
    //Inicialização dos valores padrão
    routes.put("guj", "www.guj.com.br");
    routes.put("forum", "http://www.guj.com.br/forums/list.java");
 }

 //Demais métodos
 ´´´
 ###Reference
 - [Reference #1](https://www.guj.com.br/t/qual-e-a-utilizacao-de-static/93790/2)

