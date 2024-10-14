Jetpack Compose
===============

[Jump to navigation](https://ccti.ismai.pt/android/Jetpack_Compose#mw-head)[Jump to search](https://ccti.ismai.pt/android/Jetpack_Compose#searchInput)

<-- [Voltar à página hierarquicamente anterior](https://ccti.ismai.pt/android/Main_Page "Main Page")

Contents
--------

-   [1Introdução ao Jetpack Compose](https://ccti.ismai.pt/android/Jetpack_Compose#Introdu%C3%A7%C3%A3o_ao_Jetpack_Compose)
    -   [1.1O que é o Jetpack Compose](https://ccti.ismai.pt/android/Jetpack_Compose#O_que_%C3%A9_o_Jetpack_Compose)
    -   [1.2Resolução de Problemas de Compilação (causados por bugs do Android Studio Giraffe | 2022.3.1 Patch 1 e Patch 2)](https://ccti.ismai.pt/android/Jetpack_Compose#Resolu%C3%A7%C3%A3o_de_Problemas_de_Compila%C3%A7%C3%A3o_(causados_por_bugs_do_Android_Studio_Giraffe_|_2022.3.1_Patch_1_e_Patch_2))
    -   [1.3Erro java.net.SocketException: socket failed: EPERM (Operation not permitted)](https://ccti.ismai.pt/android/Jetpack_Compose#Erro_java.net.SocketException:_socket_failed:_EPERM_(Operation_not_permitted))
    -   [1.4Tentar alterar o nome da aplicação e/ou o nome do package](https://ccti.ismai.pt/android/Jetpack_Compose#Tentar_alterar_o_nome_da_aplica%C3%A7%C3%A3o_e/ou_o_nome_do_package)
    -   [1.5Hello World em Jetpack Compose](https://ccti.ismai.pt/android/Jetpack_Compose#Hello_World_em_Jetpack_Compose)
    -   [1.6Versão do Material Design](https://ccti.ismai.pt/android/Jetpack_Compose#Vers%C3%A3o_do_Material_Design)
    -   [1.7Usar o @Preview](https://ccti.ismai.pt/android/Jetpack_Compose#Usar_o_@Preview)
-   [2Componentes gráficos básicos](https://ccti.ismai.pt/android/Jetpack_Compose#Componentes_gr%C3%A1ficos_b%C3%A1sicos)
    -   [2.1Button](https://ccti.ismai.pt/android/Jetpack_Compose#Button)
    -   [2.2stringResource](https://ccti.ismai.pt/android/Jetpack_Compose#stringResource)
    -   [2.3Text](https://ccti.ismai.pt/android/Jetpack_Compose#Text)
    -   [2.4TextField](https://ccti.ismai.pt/android/Jetpack_Compose#TextField)
    -   [2.5OutlinedTextField](https://ccti.ismai.pt/android/Jetpack_Compose#OutlinedTextField)
    -   [2.6Spacer](https://ccti.ismai.pt/android/Jetpack_Compose#Spacer)
    -   [2.7Box](https://ccti.ismai.pt/android/Jetpack_Compose#Box)
    -   [2.8Checkbox](https://ccti.ismai.pt/android/Jetpack_Compose#Checkbox)
    -   [2.9Mostrar uma mensagem (*Toast*)](https://ccti.ismai.pt/android/Jetpack_Compose#Mostrar_uma_mensagem_(Toast))
    -   [2.10Mostrar uma página web (*AndroidView*)](https://ccti.ismai.pt/android/Jetpack_Compose#Mostrar_uma_p%C3%A1gina_web_(AndroidView))
-   [3remember e mutableStateOf](https://ccti.ismai.pt/android/Jetpack_Compose#remember_e_mutableStateOf)
-   [4Layout Groups](https://ccti.ismai.pt/android/Jetpack_Compose#Layout_Groups)
    -   [4.1Row](https://ccti.ismai.pt/android/Jetpack_Compose#Row)
    -   [4.2Column](https://ccti.ismai.pt/android/Jetpack_Compose#Column)
    -   [4.3Box](https://ccti.ismai.pt/android/Jetpack_Compose#Box_2)
    -   [4.4Surface](https://ccti.ismai.pt/android/Jetpack_Compose#Surface)
    -   [4.5Scaffold](https://ccti.ismai.pt/android/Jetpack_Compose#Scaffold)
    -   [4.6ConstraintLayout](https://ccti.ismai.pt/android/Jetpack_Compose#ConstraintLayout)
    -   [4.7LazyColumn](https://ccti.ismai.pt/android/Jetpack_Compose#LazyColumn)
    -   [4.8LazyRow](https://ccti.ismai.pt/android/Jetpack_Compose#LazyRow)
    -   [4.9LazyVerticalGrid](https://ccti.ismai.pt/android/Jetpack_Compose#LazyVerticalGrid)
    -   [4.10LazyHorizontalGrid](https://ccti.ismai.pt/android/Jetpack_Compose#LazyHorizontalGrid)
    -   [4.11LazyVerticalStaggeredGrid](https://ccti.ismai.pt/android/Jetpack_Compose#LazyVerticalStaggeredGrid)
    -   [4.12LazyHorizontalStaggeredGrid](https://ccti.ismai.pt/android/Jetpack_Compose#LazyHorizontalStaggeredGrid)
-   [5Listas](https://ccti.ismai.pt/android/Jetpack_Compose#Listas)
    -   [5.1LazyColumn](https://ccti.ismai.pt/android/Jetpack_Compose#LazyColumn_2)
    -   [5.2LazyRow](https://ccti.ismai.pt/android/Jetpack_Compose#LazyRow_2)
    -   [5.3LazyColumn e LazyRow](https://ccti.ismai.pt/android/Jetpack_Compose#LazyColumn_e_LazyRow)
-   [6Modifiers](https://ccti.ismai.pt/android/Jetpack_Compose#Modifiers)
    -   [6.1Como funcionam os Modifiers](https://ccti.ismai.pt/android/Jetpack_Compose#Como_funcionam_os_Modifiers)
    -   [6.2Imports dos Modifiers](https://ccti.ismai.pt/android/Jetpack_Compose#Imports_dos_Modifiers)
    -   [6.3Lista dos principais Modifiers](https://ccti.ismai.pt/android/Jetpack_Compose#Lista_dos_principais_Modifiers)
-   [7Recursos](https://ccti.ismai.pt/android/Jetpack_Compose#Recursos)
    -   [7.1Adicionar uma imagem](https://ccti.ismai.pt/android/Jetpack_Compose#Adicionar_uma_imagem)
    -   [7.2Adicionar um ícone](https://ccti.ismai.pt/android/Jetpack_Compose#Adicionar_um_%C3%ADcone)
    -   [7.3Adicionar uma cor a colors.xml](https://ccti.ismai.pt/android/Jetpack_Compose#Adicionar_uma_cor_a_colors.xml)
    -   [7.4Adicionar um string a strings.xml](https://ccti.ismai.pt/android/Jetpack_Compose#Adicionar_um_string_a_strings.xml)
-   [8Fornecer e receber dados do interface gráfico (gerir o "estado" da App)](https://ccti.ismai.pt/android/Jetpack_Compose#Fornecer_e_receber_dados_do_interface_gr%C3%A1fico_(gerir_o_%22estado%22_da_App))
-   [9App para conversão de temperaturas Celsius - Farenheit](https://ccti.ismai.pt/android/Jetpack_Compose#App_para_convers%C3%A3o_de_temperaturas_Celsius_-_Farenheit)
    -   [9.1Imports adicionais](https://ccti.ismai.pt/android/Jetpack_Compose#Imports_adicionais)
    -   [9.2ConverterTemperatura()](https://ccti.ismai.pt/android/Jetpack_Compose#ConverterTemperatura())
    -   [9.3TextFieldTemperatura(aTemperatura: MutableState<String>, modifier: Modifier = Modifier, callback: () -> Unit)](https://ccti.ismai.pt/android/Jetpack_Compose#TextFieldTemperatura(aTemperatura:_MutableState%3CString%3E,_modifier:_Modifier_=_Modifier,_callback:_()_-%3E_Unit))
    -   [9.4ButtonGroupEscalaDeTemperatura(selecionado: MutableState<Int>, modifier: Modifier = Modifier)](https://ccti.ismai.pt/android/Jetpack_Compose#ButtonGroupEscalaDeTemperatura(selecionado:_MutableState%3CInt%3E,_modifier:_Modifier_=_Modifier))
    -   [9.5RadioButtonTemperatura(selecionado: Boolean, resId: Int, onClick: (Int) -> Unit, modifier: Modifier = Modifier)](https://ccti.ismai.pt/android/Jetpack_Compose#RadioButtonTemperatura(selecionado:_Boolean,_resId:_Int,_onClick:_(Int)_-%3E_Unit,_modifier:_Modifier_=_Modifier))
    -   [9.6Scratch](https://ccti.ismai.pt/android/Jetpack_Compose#Scratch)
-   [10Criar uma App com 4 ecrãs](https://ccti.ismai.pt/android/Jetpack_Compose#Criar_uma_App_com_4_ecr%C3%A3s)
    -   [10.1Ecras.kt](https://ccti.ismai.pt/android/Jetpack_Compose#Ecras.kt)
    -   [10.2Destinos.kt](https://ccti.ismai.pt/android/Jetpack_Compose#Destinos.kt)
    -   [10.3MainActivity.kt](https://ccti.ismai.pt/android/Jetpack_Compose#MainActivity.kt)

Introdução ao Jetpack Compose
-----------------------------

### O que é o Jetpack Compose

1.  Uma nova forma de criar o interface gráfico de uma app Android que permite que se use exclusivamente a linguagem Kotlin em todo o lado, vez de se usar Kotlin ou Java para a aplicação propriamente dita e XML para o interface gráfico
2.  No entanto apesar de se usar exclusivamente Kotlin a componente Kotlin do interface gráfico tem características especiais que é necessário tomar em linha de conta:
    1.  Usa-se quase exclusivamente funções puras (programação funcional), isto é, sem efeitos colaterais (as funções não podem por exemplo alterar o valor de uma variável global), pelo que se a mesma função for chamada com os mesmos argumentos tem obrigatoriamente que dar o mesmo resultado
    2.  Usa-se programação declarativa (em vez de programação imperativa), diz-se o que se quer em vez de como o fazer (parecido com o SQL em que se faz uma query declarando a relação entre as tabelas e os campos mas não se diz de que forma se deve proceder para obter o resultado da query)
    3.  As funções Kotlin do interface gráfico são marcadas com a anotação `@Composable`, o que, com a ajuda de um plugin para o compilador de Kotlin, altera o tipo dessas funções de modo a serem apropriadas para serem usadas no ambiente especial do interface gráfico: o que se faz é criar nós de uma árvore (a árvore com os componentes gráficos), árvore essa que é recalculada automaticamente cada vez que um componente gráfico se altera (por exemplo reagindo a uma tecla premida pelo utilizador), e de modo a ter um bom desempenho as funções são pré-calculadas, pelo que se uma dada função for chamada de novo com os mesmos argumentos usa-se simplesmente o valor já existente em cache
    4.  A ligação entre a parte *normal* da App e a componente do interface gráfico (as funções `@Composable`) faz-se usando a função `setContent()`, não é possível chamar funções marcadas como sendo `@Composable` exceto a partir daí

### Resolução de Problemas de Compilação (causados por bugs do Android Studio Giraffe | 2022.3.1 Patch 1 e Patch 2)

Já existe Android Studio Giraffe | 2022.3.1 Patch 3, ainda não foi verificado se estas bugs continuam a existir nessa versão.

1.  Erro a instalar o emulador: [instruções instalar emulator](https://github.com/google/android-emulator-hypervisor-driver)
2.  Erro de compilação com a mensagem de erro `Dependency 'androidx.activity:activity:1.8.0' requires libraries and applications that depend on it to compile against version 34 or later of the Android APIs.` Este problema parece ser causado por o Android 14 estar para ser publicado brevemente, e por alguma razão o Android Studio está a descarregar alguns ficheiros que referenciam a versão errada de algumas bibliotecas. **Solução**: abrir *Gradle Scripts / build.gradle.kts (Module:App)* e na secção *dependencies* alterar de `implementation("androidx.activity:activity-compose:1.8.0")` para `implementation("androidx.activity:activity-compose:1.7.2")` e a seguir no topo à direita carregue no *Sync Now* para sincronizar a configuração com o *build* que vai ser feito
3.  Erro de compilação com a mensagem de erro `Dependency 'androidx.emoji2:emoji2-views-helper:1.4.0' requires libraries and applications that depend on it to compile against version 34 or later of the Android APIs.`. **Solução:** abrir *Gradle Scripts / build.gradle.kts (Module:App)* e na secção *android* adicionar `compileSdkPreview = "UpsideDownCake"` e a seguir no topo à direita carregue no *Sync Now* para sincronizar a configuração com o *build* que vai ser feito
4.  Erro de compilação com a mensagem de erro `Dependency 'androidx.compose.material3:material3:1.1.2' requires libraries and applications that depend on it to compile against version 33 or later of the Android APIs.` Este problema parece ser causado por o Android 14 estar para ser publicado brevemente, e por alguma razão o Android Studio está a descarregar alguns ficheiros que referenciam a versão errada de algumas bibliotecas. **Solução**: abrir *Gradle Scripts / build.gradle.kts (Module:App)* e na secção *dependencies* alterar de `implementation("androidx.compose.material3:material3:1.1.2")` para `implementation("androidx.compose.material3:material3")` e a seguir no topo à direita carregue no *Sync Now* para sincronizar a configuração com o *build* que vai ser feito
5.  Se está a ter problemas de compilação e não tem uma referência ao BOM ([Bill of Materials](https://developer.android.com/jetpack/compose/bom)) no *Gradle Scripts / build.gradle.kts (Module:App)* na secção *dependencies*, então experimente adicionar à secção *dependencies* `implementation(platform("androidx.compose:compose-bom:2023.03.00"))`. Para ver o que contém a versão 2023.03.00 consulte [lista de versões no BOM](https://developer.android.com/jetpack/compose/bom/bom-mapping) (selecionando na lista a versão correta, neste caso 2023.03.00, atenção que em Windows não se vê a lista em Chrome e em Edge a não ser que no topo à direita se mude o idioma para Inglês, este problema não acontece no Firefox), depois no Android Studio no topo à direita carregue no *Sync Now* para sincronizar a configuração com o *build* que vai ser feito
6.  Se ao criar um *hello world* o build do projeto nunca chega a terminar (do lado esquerdo não aparecem os ficheiros do projeto, só aparece o código Kotlin na janela principal) aparentemente esperar ou fazer *build / rebuild project* não resolve o problma. Nesse caso o melhor é criar um novo projeto (normalmente à segunda tentativa funciona).
7.  Erro de compilação com a mensagem de erro `Dependency 'androidx.navigation:navigation-common:2.7.5' requires libraries and applications that depend on it to compile against version 34 or later of the Android APIs.`. **Solução**: abrir *Gradle Scripts / build.gradle.kts (Module:App)* e na secção *android* alterar de `compileSdk = 33` para `compileSdk = 34` e a seguir no topo à direita carregue no *Sync Now* para sincronizar a configuração com o *build* que vai ser feito

### Erro java.net.SocketException: socket failed: EPERM (Operation not permitted)

À partida fazer estas 3 operações deve resolver esse problema:

1.  Adicionar ao `AndroidManifest.xml` o imediatamente antes do `<application ...`:
    1.  `<uses-permission android:name="android.permission.INTERNET"/>`
    2.  `<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />`
2.  No emulador ir a "Settings" e desinstalar a app (aparentemente algo fica na cache que só se consegue resolver desinstalando a app e voltando a instalá-la)

### Tentar alterar o nome da aplicação e/ou o nome do package

1.  Não é aconselhado fazer isto, é fácil alguma coisa correr mal e gastar-se horas a tentar resolver o problema. Normalmente é preferível criar uma nova aplicação com o nome e o package corretos, a seguir criar exatamente a mesma estrutura de ficheiros e diretórios, e depois um a um (aproveitando a funcionalidade do Android Studio que permite abrir 2 projetos ao mesmo tempo, cada um deles a correr na sua janela separada) ir copiando o código de um projeto para o outro adaptando somente os imports e o resto que for necessário adaptar
2.  No entanto se a opção for alterar o nome fazer desta forma:
    1.  Clicar com o botão da direita do rato sobre o ficheiro ou diretório e selectionar "Refactor / Rename"
    2.  Fazer refactor ao nome do package (mandando alterar em todo o lado) só permite alterar o último nome e não corrige o namespace = "com.example.myapplication1" no build.gradle.kst do módulo, por isso o programa passa a dar erro de compilação (no acesso a resources) até isso ser manualmente corrigido.
    3.  Para corrigir o nomes dos diretórios intermédios no lado esquerdo no "Project" selecionar os settings (roda dentada) e desativar "Tree Appearance / Compact Middle Packages". Seguidamente fazer refactor a cada um dos diretórios intermédios.
    4.  Depois de corrigir em todo o lado é também necessário clicar com o botão da direita sobre "app" / Open Module Settings / Modules / aba "Default Config" e alterar o "Application ID".
    5.  Ver também [StackOverflow](https://stackoverflow.com/questions/16804093/rename-package-in-android-studio), [informação antiga](http://tools.android.com/tech-docs/new-build-system/applicationid-vs-packagename) e [informação mais recente](https://developer.android.com/build/configure-app-module#set_the_application_id)
    6.  Se se estiver a usar o firebase atenção que o google-services.json depende do application id (e não do package name)

### Hello World em Jetpack Compose

Selecionar *Empty Activity*, minimum SDK API 26 (Android 8.0 Oreo), build configuration language Kotlin DSL. A primeira vez que se cria uma App usando Jetpack Compose demora muito tempo a executar porque tem de descarregar da internet muitas bibliotecas, as Apps que se criar a seguir serão criadas significativamente mais rápidas.

package pt.ismai.ccti2023.myjetpackapp1
import ...
class MainActivity : ComponentActivity() {
   override fun onCreate(savedInstanceState: Bundle?) {
       super.onCreate(savedInstanceState)
       setContent {
           MyJetpackApp1Theme {
               Surface(modifier = Modifier.fillMaxSize(), color = MaterialTheme.colorScheme.background) {
                   HelloWorld("Android")
               }
           }
       }
   }
}

@Composable
fun HelloWorld(name: String, modifier: Modifier = Modifier) {
   Text(text = "Hello $name!", modifier = modifier)
}

### Versão do Material Design

O Google [material design](https://en.wikipedia.org/wiki/Material_Design) representa o estilo de desenho gráfico que vamos usar no interface gráfico das Apps Android. Existem 3 versões dessa linguagem gráfica, `material` (versão 1) introduzida pela Google em 2014, `material2` (*Material Theme*, versão 2) introduzida pela Google em 2018 (novos tipos de letra, mais espaço em branco, cantos arredondados, ícones coloridos), e `material3` (*Material You*, versão 3) introduzida pela Google em 2021 e que já se encontra maioritariamente estável (personalização efetuada pelo utilizador, cores dinâmicas em função do *wallpaper* do utilizador, outras formas, nova tipografia, botões maiores, etc.), ver por exemplo [como migrar para Material Design 3](https://material.io/blog/migrating-material-3) e a [evolução do material design](https://espeo.eu/blog/the-evolution-of-material-design/)

O que nos interessa é que ao usar `import` temos de selecionar a versão correta da biblioteca, por exemplo:

-   `import androidx.compose.material.Text`
-   `import androidx.compose.material2.Text`
-   `import androidx.compose.material3.Text`

no nosso caso iremos utilizar `material3`

### Usar o `@Preview`

Usando o `@Preview` conseguimos ter uma pré-visualização de como irá ficar o interface sem ter de o correr no emulador, o que pode ser mais rápido e liberta recursos. Por exemplo:

@Preview(showBackground = true)
@Composable
fun MyPreview() {
   MyJetpackApp1Theme {
       MyTopWidget(modifier = Modifier.fillMaxSize())
   }
}

(neste caso o `MyJetpackApp1Theme` vem do `import pt.ismai.ccti2023.myjetpackapp1.ui.theme.MyJetpackApp1Theme` num contexto em que a App chama-se `MyJetpackApp1`, o package name é `package pt.ismai.ccti2023.myjetpackapp1`, e o `Composable` que usamos dentro do `setContent()` é `MyTopWidget(...)`, isto é, temos de nos lembrar de manter o que está dentro do `setContent()` sincronizado com o que está dentro do `@Preview` senão podemos a estar a fazer preview de algo diferente do que aparece na aplicação no emulador)

Componentes gráficos básicos
----------------------------

### Button

-   Corresponde ao `Button` e ao `ImageButton` quando se faz o interface gráfico em XML
-   `import androidx.compose.material3.Button`
-   `import androidx.compose.material3.ButtonDefaults`
-   `import androidx.compose.foundation.BorderStroke`
-   `import androidx.compose.ui.unit.dp`
-   `import androidx.compose.ui.unit.sp`
-   Exemplo de utilização:

@Composable
fun MyButton() {
  Button(onClick = {}, border = BorderStroke(1.dp, color = Color.Red)) {
    Text(text = stringResource(id = R.string.button_text), color = Color.White)
  }
}

-   Assinatura completa da função: @Composable fun Button( onClick: () -> Unit, modifier: Modifier = Modifier, enabled: Boolean = true, shape: Shape = ButtonDefaults.shape, colors: ButtonColors = ButtonDefaults.buttonColors(), elevation: ButtonElevation? = ButtonDefaults.buttonElevation(), border: BorderStroke? = null, contentPadding: PaddingValues = ButtonDefaults.ContentPadding, interactionSource: MutableInteractionSource = remember { MutableInteractionSource() }, content: @Composable RowScope.() -> Unit ) { ... }
-   Argumento obrigatórios:
    1.  `onClick`: callback (normalmente uma função anónima, isto é um *[lambda](https://ccti.ismai.pt/android/FAQ_Kotlin#Kotlin_-_Express%C3%B5es_lambda "FAQ Kotlin")*) que é chamado quando o utilizador carrega no botão
    2.  `content`: conteúdo para o botão, normalmente será um `Text()`
-   Principais argumentos opcionais:
    1.  `enabled`: booleano para permitir tornar o botão ativo (valor por omissão se o argumento não for fornecido) ou inativo

### stringResource

-   É uma função *composable* que permite carregar uma string (opcionalmente formatando-a com os argumentos fornecidos) a partir do seu *resource ID* (substitui o `getString()`)
-   Pode precisar de `import androidx.compose.ui.res.stringResource`
-   Exemplos de utilização:
    1.  `Text(text = stringResource(id = R.string.etiquetaApelido))`
    2.  `Text(text = stringResource(id = R.string.helloMsgs, nome, n)`, neste caso assumindo que a variável `nome` tem o valor *Ana*, a variável `n` tem o valor 5, e `res/values/strings.xml` tem `<string name="helloMsgs">Olá, %1$s.\nTem %2$d novas mensagens.</string>` obtemos as 2 linhas de texto *Olá, Ana.<newline>Tem 5 novas mensagens.* (neste caso o `%1` refere-se ao primeiro argumento adicional e o `%2` ao segundo argumento adicional, e o `$s` define que o argumento é uma string e o `$d` que o argumento é um número inteiro, pode-se igualmente usar formatação HTML: bold *< b >...< /b>, itálico < i >...< /i>, superscript < sup>...< /sup>, subscript < sub>...< /sub>, underlined < ul>, < li>, < /ul>, etc.)*
-   Note-se que a maneira mais rápida de definir a string é declarar o id, escrevendo por exemplo `stringResource(id = R.string.etiquetaApelido)` e a seguir pairar com o cursor sobre o erro (isto é, pairar sobre `R.string.etiquetaApelido`) e premir **Alt+Shift+Enter** para abrir a janela que permite definir o `New String Value Resource`

### Text

-   Corresponde ao `TextView` quando se faz o interface gráfico em XML (texto não editável)
-   `import androidx.compose.material3.Text`
-   Exemplos de utilização:
    1.  Texto fixo: `Text(text = "O meu texto", modifier = modifier)`
    2.  Texto que inclui o valor de variáveis: `Text(text = "... $nome ...", modifier = modifier)`
    3.  O texto já se encontra numa variável: `Text(text = nome, modifier = modifier)`
    4.  Texto com formatação: `Text(text = "O meu texto", fontStyle = FontStyle.Italic, color = Color.Red, fontSize = 30.sp, fontWeight = FontWeight.Bold)`
-   Assinatura completa da função: `@Composable fun Text( text: String, modifier: Modifier = Modifier, color: Color = Color.Unspecified, fontSize: TextUnit = TextUnit.Unspecified, fontStyle: FontStyle? = null, fontWeight: FontWeight? = null, fontFamily: FontFamily? = null, letterSpacing: TextUnit = TextUnit.Unspecified, textDecoration: TextDecoration? = null, textAlign: TextAlign? = null, lineHeight: TextUnit = TextUnit.Unspecified, overflow: TextOverflow = TextOverflow.Clip, softWrap: Boolean = true, maxLines: Int = Int.MAX_VALUE, onTextLayout: (TextLayoutResult) -> Unit = {}, style: TextStyle = LocalTextStyle.current ) { ... }`
-   Principais argumentos opcionais:
    1.  `color`: a cor do texto, por exemplo para texto vermelho com 30% de transparência (70% de opacidade) usa-se `Color(red = 1f, green = 0f, blue = 0f, alpha = 0.7f)`
    2.  `fontSize`: o tamanho do texto mede-se em *scalable pixels* (**sp**), por exemplo para tamanho 20 usa-se `20.sp`
    3.  `fontStyle`: o tipo de letra pode ser normal ou itálico, por exemplo para itálico usa-se `Italic`
    4.  `fontWeight`: o *peso* da letra, por exemplo para negrito usa-se `FontWeight.Bold`
    5.  `maxLines`: número máximo de linhas que o texto pode ocupar
    6.  `overflow`: o que fazer quando o texto é longo demais, por exemplo para aparecerem reticências usa-se `Ellipsis` (usa-se `Clip` para truncar o texto)

### TextField

-   Corresponde ao `EditText` quando se faz o interface gráfico em XML (texto editável)
-   `import androidx.compose.material3.TextField`
-   `import androidx.compose.runtime.mutableStateOf`
-   `import androidx.compose.runtime.remember`
-   Campo de texto editável armazenado numa variável, temos de ter cautela sobre como o fazer porque necessitamos de usar funções puras, daí a necessidade do `remember` e do `mutableStateOf`:
-   Exemplo de utilização (neste exemplo é impossível usar o valor colocado no campo pelo que é um exemplo simples mas pouco interessante):

@Composable
fun MyTextField() {
  val valorDoCampo = remember { mutableStateOf("") }
  TextField(value = valorDoCampo.value, onValueChange = { valorDoCampo.value = it }, label = {})
}

-   Exemplo mais complexo para ler um número em que o valor colocado no campo pode ser usado por quem chamar esta função e em que se esconde o teclado quando se termina de introduzir o valor:

@Composable
fun TextFieldNumero(oCampo: MutableState<String>, callback: () -> Unit, modifier: Modifier = Modifier) {
   val keyboardController = LocalSoftwareKeyboardController.current // usado para esconder o teclado quando se termina
   TextField(value = oCampo.value, onValueChange = { oCampo.value = it },
       placeholder = { Text(text = stringResource(id = R.string.numeroPlaceholder)) },
       modifier = modifier,
       keyboardActions = MyKeyboardActions(onAny = { callback() }, onDone = { keyboardController?.hide() } ),
       keyboardOptions = KeyboardOptions(keyboardType = KeyboardType.Number, imeAction = ImeAction.Done),
       singleLine = true
   )
}
// função copiada e adaptada do código fonte do androidx.compose.foundation.text.KeyboardActions.kt, permite executar lambdas diferentes consoante se altera o valor ou se termina a introdução do valor:
fun MyKeyboardActions(onAny: KeyboardActionScope.() -> Unit, onDone:KeyboardActionScope.() -> Unit ): KeyboardActions = KeyboardActions(
   onDone = onDone, onGo = onAny, onNext = onAny, onPrevious = onAny, onSearch = onAny, onSend = onAny
)

-   Assinatura completa da função: `@ExperimentalMaterial3Api @Composable fun TextField( value: String, onValueChange: (String) -> Unit, modifier: Modifier = Modifier, enabled: Boolean = true, readOnly: Boolean = false, textStyle: TextStyle = LocalTextStyle.current, label: @Composable (() -> Unit)? = null, placeholder: @Composable (() -> Unit)? = null, leadingIcon: @Composable (() -> Unit)? = null, trailingIcon: @Composable (() -> Unit)? = null, supportingText: @Composable (() -> Unit)? = null, isError: Boolean = false, visualTransformation: VisualTransformation = VisualTransformation.None, keyboardOptions: KeyboardOptions = KeyboardOptions.Default, keyboardActions: KeyboardActions = KeyboardActions.Default, singleLine: Boolean = false, maxLines: Int = Int.MAX_VALUE, interactionSource: MutableInteractionSource = remember { MutableInteractionSource() }, shape: Shape = TextFieldDefaults.filledShape, colors: TextFieldColors = TextFieldDefaults.textFieldColors() ) { ... }`
-   Argumento obrigatórios:
    1.  `value`: é do tipo `TextFieldValue`, não é um `String`
    2.  `onValueChange`: callback (normalmente uma função anónima, isto é um *[lambda](https://ccti.ismai.pt/android/FAQ_Kotlin#Kotlin_-_Express%C3%B5es_lambda "FAQ Kotlin")*) que é chamado quando o utilizador carrega numa tecla, o callback fornece um novo `TextFieldValue` que pode ser usado para atualizar o valor do campo
-   Principais argumentos opcionais:
    1.  `label`: a etiqueta que é mostrada dentro do contentor, quando o utilizador coloca o foco no texto a etiqueta é objeto de uma animação
    2.  `keyboardOptions`: permite definir o `KeyboardType` (por exemplo `Email`, `Password`, `Number`) e a `[ImeAction](https://proandroiddev.com/androids-ime-actions-don-t-ignore-them-36554da892ac)` (Input Method Editor Action, por exemplo `Go`, `Search`, `Previous`, `Next`, `Done` de modo a dar um melhor feedback ao utilizador relativamente ao que está a ser efetuado)
    3.  `keybardAction`: permite definir callbacks para `ImeActions`
    4.  `enabled`: booleano para permitir tornar o campo ativo (valor por omissão se o argumento não for fornecido) ou inativo
    5.  `readOnly`: booleano para permitir tornar o campo de leitura e escrita (valor por omissão se o argumento não for fornecido) ou só de leitura

### OutlinedTextField

-   É um `TextField` mais sofisticado do ponto de vista gráfico que permite ter um contorno animado à volta do campo (texto editável)
-   `import androidx.compose.material3.OutlinedTextField`
-   `import androidx.compose.runtime.mutableStateOf`
-   `import androidx.compose.runtime.remember`
-   Campo de texto editável armazenado numa variável, temos de ter cautela sobre como o fazer porque necessitamos de usar funções puras, daí a necessidade do `remember` e do `mutableStateOf`
-   Exemplo de utilização assumindo que em `res / values / strings.xml` existe `<string name="etiquetaEmail">Email</string>`

@Composable
fun MyOutlinedTextField() {
   val textValue = remember { mutableStateOf("avs@ismai.pt") }
   val primaryColor1 = Color(red = 0f, green = 0f, blue = 1f, alpha = 1f)
   val primaryColor2 = Color(red = 0f, green = 1f, blue = 0f, alpha = 1f)
   OutlinedTextField(
       label = { Text(text = stringResource(id = R.string.etiquetaEmail)) },
       colors = TextFieldDefaults.outlinedTextFieldColors(
           focusedBorderColor = primaryColor1,
           focusedLabelColor = primaryColor2,
           cursorColor = primaryColor1
       ),
       keyboardOptions = KeyboardOptions.Default.copy(keyboardType = KeyboardType.Email),
       value = textValue.value,
       onValueChange = {textValue.value = it },
   )
}

outras opções possíveis para o *keyboardType* (relevantes dependendo do contexto) seriam `KeyboardType.Number`, `KeyboardType.Password`, `KeyboardType.Phone`, `KeyboardType.Uri`, `KeyboardType.NumberPassword.Text`

-   Assinatura completa da função: `@ExperimentalMaterial3Api @Composable fun OutlinedTextField( value: String, onValueChange: (String) -> Unit, modifier: Modifier = Modifier, enabled: Boolean = true, readOnly: Boolean = false, textStyle: TextStyle = LocalTextStyle.current, label: @Composable (() -> Unit)? = null, placeholder: @Composable (() -> Unit)? = null, leadingIcon: @Composable (() -> Unit)? = null, trailingIcon: @Composable (() -> Unit)? = null, supportingText: @Composable (() -> Unit)? = null, isError: Boolean = false, visualTransformation: VisualTransformation = VisualTransformation.None, keyboardOptions: KeyboardOptions = KeyboardOptions.Default, keyboardActions: KeyboardActions = KeyboardActions.Default, singleLine: Boolean = false, maxLines: Int = Int.MAX_VALUE, interactionSource: MutableInteractionSource = remember { MutableInteractionSource() }, shape: Shape = TextFieldDefaults.outlinedShape, colors: TextFieldColors = TextFieldDefaults.outlinedTextFieldColors() ) { ... }`

### Spacer

-   Separador para colocar espaço adicional entre componentes
-   `import androidx.compose.foundation.layout.Spacer`
-   `import androidx.compose.foundation.layout.height`
-   `import androidx.compose.foundation.layout.width`
-   Exemplo de utilização: `Spacer(modifier = Modifier.height(38.dp))`
-   Assinatura completa da função: `@Composable @NonRestartableComposable fun Spacer(modifier: Modifier) { ... }`

### Box

-   Existem 2 versões do `Box`, a que funciona como um [layout](https://ccti.ismai.pt/android/Jetpack_Compose#Box_2) e a que funciona como uma primitiva (para por exemplo desenhar um quadrado, retângulo ou círculo) se não tiver elementos no seu interior e forem fornecidos somente *modifiers*
-   Assinatura completa da função quando funciona como uma primitiva: `@Composable fun Box(modifier: Modifier) { Layout({}, measurePolicy = EmptyBoxMeasurePolicy, modifier = modifier) }`
-   Alterando somente o *modifier* pode igualmente ser usado para criar um quadrado com uma dada cor e tamanho `Box(modifier = Modifier.background(Color.Black).size(30.dp))` ou um retângulo com uma dada cor e tamanho `Box(modifier = Modifier.background(Color.Black).size(30.dp, 10.dp))` ou um círculo com uma dada cor e tamanho `Box(modifier = Modifier.clip(CircleShape).background(Color.Black).size(30.dp))`

### Checkbox

-   Permite adicionar uma checkbox que pode ou não já vir preenchida
-   Exemplo de utilização: `Checkbox(checked = false, onCheckedChange = { }, modifier = Modifier.padding(8.dp))`
-   Assinatura completa da função: `@Composable fun Checkbox(checked: Boolean, onCheckedChange: ((Boolean) -> Unit)?, modifier: Modifier = Modifier, enabled: Boolean = true, interactionSource: MutableInteractionSource = remember { MutableInteractionSource() }, colors: CheckboxColors = CheckboxDefaults.colors() ) { ... }`
-   Como a checkbox não inclui suporte para se fornecer a etiqueta com o texto descritivo pode-se criar a função `CheckboxComEtiqueta()` que já faz isso:

@Composable
fun CheckboxComEtiqueta(etiqueta: String, state: MutableState<Boolean>) {
   Row(modifier = Modifier.clickable { state.value = !state.value }, verticalAlignment = Alignment.CenterVertically) {
      Checkbox(checked = state.value, onCheckedChange = { state.value = it })
      Text(text = etiqueta, modifier = Modifier.padding(start = 8.dp))
   }
}

para usar esta função basta declarar na função que chama esta algo de semelhante a `val cState: MutableState<Boolean> = remember { mutableStateOf(false) }` e depois chamar usando algo de semelhante a `CheckboxComEtiqueta("Concordo com as regras", cState)`

### Mostrar uma mensagem (*Toast*)

-   Em Android uma mensagem temporária (que aparece e desaparece pouco tempo depois) é mostrada usando um *Toast*
-   O *toast* tem o seguinte formato: `Toast.makeText(oContexto, aMensagem, Toast.LENGTH_SHORT).show()`, em que `oContexto` é o contexto em que a mensagem deve aparecer (ver abaixo) e `aMensagem` é uma string, pode-se igualmente usar `Toast.LENGTH_LONG` mas normalmente isso faz com que a mensagem seja visível durante um tempo excessivo
-   A mensagem tem de ser mostrada num dado contexto, para isso dentro de um *composable* declaramos `val oContexto = LocalContext.current`

### Mostrar uma página web (*AndroidView*)

1.  No `AndroidManifest.xml` imediatamente antes do `<application ...` adicionar

 <uses-permission android:name="android.permission.INTERNET"/>
 <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />

1.  Adicionar estes "imports"

import android.webkit.WebView
import android.webkit.WebViewClient

1.  Criar uma função semelhante a esta

@Composable
fun WebViewScreen(url: String) {
   AndroidView(
       factory = { context ->
           WebView(context).apply {
               settings.javaScriptEnabled = true
               webViewClient = WebViewClient()
               settings.loadWithOverviewMode = true
               settings.useWideViewPort = true
               settings.setSupportZoom(true)
           }
       },
       update = { webView -> webView.loadUrl(url)
       }
   )
}

1.  Chamar a função com, por exemplo `WebViewScreen("[https://www.ipmaia.pt](https://www.ipmaia.pt/)")`
2.  Ao correr no emulador pode ser necessário resolver problemas de acesso à internet:
    1.  Verificar que no emulador o WiFi está ativado
    2.  Se ocorrer `net::ERR_NAME_NOT_RESOLVED` então será necessário configurar o DNS

remember e mutableStateOf
-------------------------

-   `remember` e `mutableStateOf` são conceitos completamente independentes entre si embora costumem ser usados em conjunto
-   `remember` permite que um valor (qualquer tipo de valor) possa ser mantido (não perdido) ao se aplicar recomposições. `remember` é uma função *composable* que *memoizes* (calcula e armazena o valor numa cache) o valor devolvido pela função anónima (lambda) passada a ela e devolve esse valor, desta forma permitindo que não se perca o valor de variáveis que sejam alteradas quando se fazem recomposições. A primeira vez que se chama `remember` executa o lambda para obter esse valor e armazena (*memoizes*) esse valor. A próxima vez que o *composable* é recalculado a chamada ao *remember* irá ver se já existe um valor armazenado da vez anterior e se sim devolve-o sem chamar o lambda. Pode-se *lembrar* qualquer tipo de valor, primitivas ou classes, uma das coisas que se pode *lembrar* é o tipo *MutableState*, mas não existe nada de especial na relação com esse tipo. Note-se que só se pode usar *remember* dentro de funções *composable* (o compilador irá queixar-se se isso for feito fora dessas funções)
-   `mutableStateOf` devolve um `MutableState` (pensar por exemplo no `mutableListOf` do Kotlin), um `MutableState` permite armazenar um valor de tal forma que o Compose é informado automaticamente das alterações que sejam efetuadas a esse valor
-   Ao nível do programa principal as variáveis que se pretende sejam passadas a funções composable chamadas a partir desse programa principal devem ser declaradas como sendo, por exemplo:
    1.  `val preco = remember { mutableStateOf(0.0F) }`
    2.  `val nome = remember { mutableStateOf("") }`

    e depois ao chamar as funções composable fornece-se como argumento `preco` ou `nome` sendo que quando quer nessas funções quer no programa principal se pretende obter ou alterar o valor da variável tem de se usar `preco.value` ou `nome.value`

Layout Groups
-------------

### Row

-   Corresponde à versão *horizontal* do `LinearLayout` quando se faz o interface gráfico em XML
-   `import androidx.compose.foundation.layout.Row`
-   `import androidx.compose.ui.Alignment`
-   `import androidx.compose.foundation.layout.Arrangement`
-   Exemplo de utilização com um campo de texto e um botão usando a função `MyOutlinedTextField()`definida em [OutlinedTextField](https://ccti.ismai.pt/android/Jetpack_Compose#OutlinedTextField) e a função `MyButton()`definida em [Button](https://ccti.ismai.pt/android/Jetpack_Compose#Button)

@Composable
fun MyRow() {
   Row(verticalAlignment = Alignment.CenterVertically,
       horizontalArrangement = Arrangement.SpaceEvenly,
       modifier = Modifier.fillMaxSize()) {
           MyOutlinedTextField()
           MyButton()
       }
}

-   Assinatura completa da função: `@Composable inline fun Row( modifier: Modifier = Modifier, horizontalArrangement: Arrangement.Horizontal = Arrangement.Start, verticalAlignment: Alignment.Vertical = Alignment.Top, content: @Composable RowScope.() -> Unit ) { ... }`
-   Argumento obrigatórios:
    1.  `content`: os filhos a colocar horizontalmente dentro do layout
-   Principais argumentos opcionais:
    1.  `horizontalArrangement`: como distribuir o espaço disponível na horizontal (`Arrangement.SpaceBetween` cada elemento fica com a mesma quantidade de espaço sem incluir espaço antes do primeiro nem depois do último, `Arrangement.SpaceEvenly` idem mas incluindo espaço antes do primeiro e depois do último, `Arrangement.SpaceAround` idem mas reduzindo para metade o espaço entre filhos consecutivos, `Arrangement.Center` `Arrangement.Start` ou `Arrangement.End` para não colocar espaço entre os filhos)
    2.  `verticalAlignment`: como alinhar os filhos na vertical (`Alignment.Top` é o valor por omissão que alinha no topo, `Alignment.CenterVertically` alinha ao centro, `Alignment.Bottom` alinha no fundo)
    3.  `modifier`: usar `Modifier.fillMaxSize()` se quisermos ocupar todo o espaço disponível
-   Pode-se também posicionar os filhos dentro do layout dando-lhes pesos diferentes, por exemplo `Text(modifier = Modifier.weight(2/3f), ...)` e `Button(modifier = Modifier.weight(1/3f), ...)`

### Column

-   Corresponde à versão *vertical* do `LinearLayout` quando se faz o interface gráfico em XML
-   `import androidx.compose.foundation.layout.Column`
-   `import androidx.compose.ui.Alignment`
-   `import androidx.compose.foundation.layout.Arrangement`
-   Exemplo de utilização com um campo de texto e um botão usando a função `MyOutlinedTextField()`definida em [OutlinedTextField](https://ccti.ismai.pt/android/Jetpack_Compose#OutlinedTextField) e a função `MyButton()`definida em [Button](https://ccti.ismai.pt/android/Jetpack_Compose#Button)

@Composable
fun MyColumn() {
   Column(horizontalAlignment = Alignment.CenterHorizontally,
       verticalArrangement = Arrangement.SpaceEvenly,
       modifier = Modifier.fillMaxSize()) {
           MyOutTextField()
           MyButton()
       }
}

-   Assinatura completa da função: `@Composable inline fun Column( modifier: Modifier = Modifier, verticalArrangement: Arrangement.Vertical = Arrangement.Top, horizontalAlignment: Alignment.Horizontal = Alignment.Start, content: @Composable ColumnScope.() -> Unit ) { ... }`
-   Argumento obrigatórios:
    1.  `content`: os filhos a colocar verticalmente dentro do layout
-   Principais argumentos opcionais:
    1.  `verticalArrangement`: como distribuir o espaço disponível na vertical (`Arrangement.SpaceBetween` cada elemento fica com a mesma quantidade de espaço sem incluir espaço antes do primeiro nem depois do último, `Arrangement.SpaceEvenly` idem mas incluindo espaço antes do primeiro e depois do último, `Arrangement.SpaceAround` idem mas reduzindo para metade o espaço entre filhos consecutivos, `Arrangement.Center` `Arrangement.Start` ou `Arrangement.End` para não colocar espaço entre os filhos)
    2.  `horizontalAlignment`: como alinhar os filhos na horizontal (`Alignment.Top` é o valor por omissão que alinha no topo, `Alignment.Center` alinha ao centro, `Alignment.Bottom` alinha no fundo)
    3.  `modifier`: usar `Modifier.fillMaxSize()` se quisermos ocupar todo o espaço disponível
-   Pode-se também posicionar os filhos dentro do layout dando-lhes pesos diferentes, por exemplo `Text(modifier = Modifier.weight(2/3f), ...)` e `Button(modifier = Modifier.weight(1/3f), ...)`

### Box

-   Existem 2 versões do `Box`, a que funciona como um layout e a que funciona como uma [primitiva](https://ccti.ismai.pt/android/Jetpack_Compose#Box) se não tiver elementos no seu interior mas somente *modifiers*
-   Se tiver elementos dentro é um layout que corresponde ao `FrameLayout` quando se faz o interface gráfico em XML, permite colocar os filhos relativamente aos limites dos seus pais e permite colocar os filhos uns por cima dos outros (útil quando se tem elementos que têm de ser colocados nesses locais específicos ou quando se tem elementos que devem ficar sobrepostos, como por exemplo diálogos)
-   `import import androidx.compose.foundation.layout.Box`
-   `import androidx.compose.ui.unit.sp`
-   `import androidx.compose.ui.unit.dp`
-   Exemplo de utilização com 3 campos de texto (assume a existência de 3 strings `primeiro segundo terceiro` definidos no res / values / strings.xml):

@Composable
fun MyBox(modifier: Modifier = Modifier, contentModifier: Modifier = Modifier) {
   Box(modifier = modifier.fillMaxSize()) {
       Text(
           text = stringResource(id = R.string.primeiro),
           fontSize = 22.sp,
           modifier = contentModifier.align(Alignment.TopStart)
       )
       Text(
           text = stringResource(id = R.string.segundo),
           fontSize = 22.sp,
           modifier = contentModifier.align(Alignment.Center)
       )
       Text(
           text = stringResource(id = R.string.terceiro),
           fontSize = 22.sp,
           modifier = contentModifier.align(Alignment.BottomEnd)
       )
   }
}

-   Assinatura completa da função: `@Composable inline fun Box( modifier: Modifier = Modifier, contentAlignment: Alignment = Alignment.TopStart, propagateMinConstraints: Boolean = false, content: @Composable BoxScope.() -> Unit ) { ... }`
-   Argumento obrigatórios:
    1.  `content`: os filhos a colocar dentro do layout
-   Principais argumentos opcionais:
    1.  `contentAlignment`: como alinhar o filho face a um dos cantos do ecrã ou face ao centro, `Alignment.TopStart`, `Alignment.TopCenter`, `Alignment.TopEnd`, `Alignment.CenterStart`, `Alignment.Center`, `Alignment.CenterEnd`, `Alignment.BottomStart`, `Alignment.BottomCenter`, `Alignment.BottomEnd`

### Surface

-   Só pode ter um único filho, permite aplicar diversos estilos a esse filho (elevação, cor, contorno, forma usada para fazer *clipping* do filho, etc.)
-   `import androidx.compose.material3.Surface`
-   `import androidx.compose.foundation.layout.size`
-   Exemplo de utilização para aplicar estilos ao `MyBox()`:

@Composable
fun MySurface(modifier: Modifier) {
   Surface(
       modifier = modifier.size(100.dp),
       color = Color.LightGray,
       contentColor = Color.Black,
       shadowElevation = 1.dp,
       border = BorderStroke(1.dp, Color.Black)
   ) {
       MyBox()
   }
}

-   Assinatura completa da função: `@Composable @NonRestartableComposable fun Surface( modifier: Modifier = Modifier, shape: Shape = RectangleShape, color: Color = MaterialTheme.colorScheme.surface, contentColor: Color = contentColorFor(color), tonalElevation: Dp = 0.dp, shadowElevation: Dp = 0.dp, border: BorderStroke? = null, content: @Composable () -> Unit ) { ... }`

### Scaffold

-   Novo layout do Jetpack Compose
-   Permite implementar um layout visual de acordo com o *Material Design* combinando diferentes elementos para obter um ecrã completo
-   Serve por exemplo para criar uma App com uma *bottom navigation bar*, ver por exemplo [app com 4 ecrãs](https://ccti.ismai.pt/android/Jetpack_Compose#Criar_uma_App_com_4_ecr%C3%A3s)

### ConstraintLayout

-   Corresponde ao ConstraintLayout quando se faz o interface gráfico em XML, permite colocar componentes no ecrã relativamente à posição dos outros componentes (alternativa ao uso de múltiplos Row, Column, Box encadeados uns dentro dos outros, útil quando se está a fazer layouts com alinhamentos complicados)

### LazyColumn

Ver [LazyColumn](https://ccti.ismai.pt/android/Jetpack_Compose#LazyColumn_2)

### LazyRow

Ver [LazyRow](https://ccti.ismai.pt/android/Jetpack_Compose#LazyRow_2)

### LazyVerticalGrid

-   Permite colocar os filhos numa grelha vertical (os filhos são colocados de modo a poder-se fazer *scroll* na vertical das diferentes colunas, todos os itens têm a mesma altura)

### LazyHorizontalGrid

-   Permite colocar os filhos numa grelha horizontal (os filhos são colocados de modo a poder-se fazer *scroll* na horizontal das diferentes linhas, todos os itens tem a mesma largura)

### LazyVerticalStaggeredGrid

-   Permite colocar os filhos numa grelha vertical (os filhos são colocados de modo a poder-se fazer *scroll* na vertical das diferentes colunas e os itens individuais podem ter diferentes alturas)

### LazyHorizontalStaggeredGrid

-   Permite colocar os filhos numa grelha horizontal (os filhos são colocados de modo a poder-se fazer *scroll* na horizontal das diferentes colunas e os itens individuais podem ter diferentes larguras)

Listas
------

### LazyColumn

-   Semelhante ao Column mas somente os elementos que são visíveis no ecrã são calculados, quando se faz *scroll* os elementos que aparecem no ecrã são calculados e os elementos que saiem do ecrã são destruídos (ao contrário do `RecyclerView` que era usado quando os interfaces eram feitos em XML os elements que desaparecem do ecrã não são reusados para criar os novos elementos, isso porque o processo de recomposição no Jetpack Compose é mais eficiente)

### LazyRow

-   Semelhante ao Row mas somente os elementos que são visíveis no ecrã são calculados, quando se faz *scroll* os elementos que aparecem no ecrã são calculados e os elementos que saiem do ecrã são destruídos (ao contrário do `RecyclerView` que era usado quando os interfaces eram feitos em XML os elements que desaparecem do ecrã não são reusados para criar os novos elementos, isso porque o processo de recomposição no Jetpack Compose é mais eficiente)

### LazyColumn e LazyRow

import androidx.annotation.StringRes
import androidx.compose.foundation.Image
import androidx.compose.ui.res.painterResource
import androidx.compose.foundation.lazy.LazyColumn
import androidx.compose.foundation.lazy.LazyRow
import androidx.compose.ui.text.font.FontWeight
import androidx.compose.foundation.layout.height
import androidx.compose.foundation.layout.Spacer
import androidx.compose.ui.layout.ContentScale
import androidx.compose.ui.res.stringResource
import androidx.compose.foundation.lazy.items

Cria-se dois composable `MinhaLista()` e `ItemDaLista()`

data class CategoriaLivro(@StringRes val categoryResourceId: Int, val recursosImagensLivros: List<Int>)

@Composable
fun ImagemLivro(imageResource: Int) {
  Image(modifier = Modifier.size(170.dp, 200.dp), painter = painterResource(id = imageResource), contentScale = ContentScale.Fit, contentDescription = stringResource(R.string.imagem_livro))
}

private val items = listOf(
 CategoriaLivro(
   R.string.titulo1,
   listOf(R.drawable.imagem1, R.drawable.imagem2, R.drawable.imagem3)
 ),
 CategoriaLivro(
   R.string.titulo2,
   listOf(R.drawable.imagem4, R.drawable.imagem5)
 ),
 CategoriaLivro(
   R.string.titulo3,
   listOf(R.drawable.imagem6, R.drawable.imagem7, R.drawable.imagem8)
 ),
 CategoriaLivro(
   R.string.titulo4,
   listOf(R.drawable.imagem9, R.drawable.imagem10)
 )
)

@Composable
fun MinhaLista() {
  LazyColumn {
    items(items) { item -> ItemDaLista(item) }
  }
}

@Composable
fun ItemDaLista(categoriaLivro: CategoriaLivro, modifier: Modifier = Modifier) {
   Column(modifier = Modifier.padding(4.dp)) {
    Text(text = "Título", fontSize = 22.sp, fontWeight = FontWeight.Bold, color = Color.Red)
    Spacer(modifier = modifier.height(4.dp))
    LazyRow {
      items(categoriaLivro.recursosImagensLivros) { items -> ImagemLivro(items) }
    }
  }
}

Modifiers
---------

### Como funcionam os Modifiers

Os *modifiers' definem como um componente gráfico se posiciona, visualiza ou comporta dentro do layout que o envolve*

Os componentes gráficos possuem o argumento `modifier: Modifier = Modifier`, trata-se de um argumento que por omissão (se não for fornecido) é inicializado com '*Modifier* que representa um *modifier vazio* pelo que herda o `Modifier` do nível envolvente, se for fornecido é alterado de acordo com o que for fornecido

Uma chamada a um *modifier* devolve um *modifier*, pelo que para tornar o código mais compacto se pode encadear os modifiers: `modifier = Modifier.opcao1(...).opcao2(...).opcao3(...)`

### Imports dos Modifiers

import androidx.compose.foundation.BorderStroke
import androidx.compose.foundation.background
import androidx.compose.foundation.border
import androidx.compose.foundation.clickable
import androidx.compose.foundation.horizontalScroll
import androidx.compose.foundation.layout.fillMaxHeight
import androidx.compose.foundation.layout.fillMaxSize
import androidx.compose.foundation.layout.fillMaxWidth
import androidx.compose.foundation.layout.heightIn
import androidx.compose.foundation.layout.padding
import androidx.compose.foundation.layout.size
import androidx.compose.foundation.rememberScrollState
import androidx.compose.foundation.shape.CircleShape
import androidx.compose.foundation.shape.RoundedCornerShape
import androidx.compose.foundation.verticalScroll
import androidx.compose.ui.Alignment
import androidx.compose.ui.Modifier
import androidx.compose.ui.draw.clip
import androidx.compose.ui.draw.shadow
import androidx.compose.ui.graphics.Color
import androidx.compose.ui.graphics.SolidColor
import androidx.compose.ui.res.stringResource
import androidx.compose.ui.unit.dp
import androidx.compose.ui.unit.sp

NOTA: o `Modifier.weight(...)` pode ser colocado dentro de um `Column()` ou dentro de um `Row()` que, consoante o caso, necessita de `import androidx.compose.foundation.layout.Column` ou `import androidx.compose.foundation.layout.Row`, mas o `Modifier.weight(...)` propriamente dito não necessita de um *import*

### Lista dos principais Modifiers

A lista completa dos modifiers existentes pode ser consultada em [List of Compose modifiers](https://developer.android.com/jetpack/compose/modifiers-list)

1.  `Modifier.size(99.dp)` configura a largura e a altura para ser essa quantidade de pixeis em *dp* (density-independent pixels)
2.  `Modifier.size(50.dp, 25.dp)` configura a largura para ser 50 pixeis e a altura para ser 25 pixeis em *dp* (density-independent pixels)
3.  `Modifier.fillMaxWidth()` ocupar a largura máxima disponível (atenção que se existirem componentes que venham depois deste na horizontal podem ficar escondidos)
4.  `Modifier.fillMaxWidth(0.8f)` ocupar 80% da largura máxima disponível
5.  `Modifier.fillMaxHeight()` ocupar a altura máxima disponível (atenção que se existirem componentes que venham depois deste na vertical podem ficar escondidos)
6.  `Modifier.fillMaxHeight(0.3f)` ocupar 30% da altura máxima disponível
7.  `Modifier.fillMaxSize()` ocupar a altura e a largura máximas disponíveis (atenção que se existirem componentes que venham depois deste na horizontal ou na vertical podem ficar escondidos)
8.  `Modifier.fillMaxSize(0.7f)` ocupar 70% da altura e 70% da largura máximas disponíveis
9.  `Modifier.weight(1f)` especifica o peso relativo do componente face aos restantes (os componentes com pesos atribuídos têm tendência para ocupar o espaço livre em função dos seus pesos relativos enquanto que os componentes sem peso atribuído ficam com o espaço mínimo). NOTA: nunca usar peso `0f`, isso faz com que o *preview* não mostre nada e a aplicação faça crash
10. `Modifier.heightIn(min=64.dp)` restringe a altura do componente a ter pelo menos o tamanho mínimo de 64 pixéis (pode-se igualmente especificar o `max`)
11. `Modifier.background(Color.Red)` pinta com essa cor o *background* do objeto gráfico
12. `Modifier.shadow(2.dp, RoundedCornerShape(8.dp))` aplica um efeito de sombra, neste caso a elevação são 2 pixéis e a forma são cantos arredondados com um raio de 8 pixéis
13. `Modifier.padding(4.dp)` coloca 4 pixeis de espaço em branco à volta do componente
14. `Modifier.padding(start=8.dp, top=4.dp, bottom=12.dp, end=2.dp)` coloca 8 pixéis à esquerda, 4 pixéis no topo, 12 pixéis no fundo, e 2 pixéis à direita (de espaço em branco à volta do componente)
15. NOTA: normalmente queremos aplicar o `padding` antes de aplicar o `size` de modo ao objeto ficar com tamanho *size*, se fizermos na ordem inversa o objeto vai ser reduzido do tamanho do *padding*
16. `Modifier.align(Alignment.CenterVertically)` alinha verticalmente ao centro (outras opções do *Alignment*: `CenterHorizontally`, `Start`, `Center`, `End`, `Bottom`, `Top`, `BottomCenter`, `BottomEnd`, `BottomStart`, `CenterEnd`, `CenterStart`, `TopCenter`, `TopEnd`, `TopStart`)
17. `Modifier.clip(CircleShape)` recorta o *conteúdo* usando um círculo (isto é, torna o objeto redondo)
18. `Modifier.clickable{...}` adiciona, aos componentes que normalmente não o necessitam, suporte para reagir a clicks (executando o lambda que se fornecer como argumento), isto permite por exemplo tornar um `Text()` clicável
19. `Modifier.border(BorderStroke(2.dp, SolidColor(Color.Black)), CircleShape)` cria um contorno circular com uma dada espessura, cor e forma
20. Exemplo de criar um contorno preto com 2 pixéis de espessura à volta de um retângulo vermelho: `Modifier.size(50.dp, 25.dp).background(Color.Red).border(BorderStroke(2.dp, SolidColor(Color.Black)))`
21. Exemplo de criar um contorno preto com 2 pixéis de espessura à volta de um círculo vermelho de diâmetro 20: `Modifier.size(20.dp).clip(CircleShape).background(Color.Red).border(BorderStroke(2.dp, SolidColor(Color.Black)), CircleShape)`
22. [![](https://ccti.ismai.pt/and/images/1/10/Column-with-3boxes-with-modifiers.png)](https://ccti.ismai.pt/android/File:Column-with-3boxes-with-modifiers.png)

    É importante aplicar os *modifiers* na ordem correta (isto é, a ordem em que eles são aplicados tem influência no resultado), por exemplo aqui o efeito do vermelho no primeiro objeto é nenhum (não se nota um círculo vermelho sobre um retângulo vermelho)`

    Column() {
           Box(modifier = Modifier.size(50.dp, 25.dp).background(Color.Red).clip(CircleShape))
           Box(modifier = Modifier.size(60.dp).background(Color.Blue).clip(CircleShape).background(Color.Yellow))
           Box(modifier = Modifier.clip(CircleShape).background(Color.Black).size(30.dp))
    }

    `
23. Se ao criarmos um componente quisermos estabelecer valores por omissão para os *modifiers* mas ao mesmo tempo permitir a quem o usar de definir para alguns dos *modifiers* outros valores fazemos desta forma (note-se que optamos por definir que `tamanho` é um argumento obrigatório, isto é, não possui valor por omissão):

[![](https://ccti.ismai.pt/and/images/0/00/Column-with-3boxes-with-modifiers-with-args.png)](https://ccti.ismai.pt/android/File:Column-with-3boxes-with-modifiers-with-args.png)

@Composable
fun CirculosQuadrados(tamanho: Dp, cor1: Color = Color.Red, cor2: Color = Color.Blue, cor3: Color = Color.Yellow, padding: Dp = 0.dp) {
   Column() {
       Box(modifier = Modifier.padding(padding).size(tamanho, tamanho / 2).background(cor1).clip(CircleShape))
       Box(modifier = Modifier.padding(padding).size(tamanho + 10.dp).background(cor2).clip(CircleShape).background(cor3))
       Box(modifier = Modifier.padding(padding).clip(CircleShape).background(Color.Black).size(tamanho / 2 + 10.dp))
   }
}
@Preview
@Composable
fun CirculosQuadradosPreview() {
   // CirculosQuadrados(tamanho = 50.dp) // aqui só são fornecidos os argumentos obrigatórios
   CirculosQuadrados(tamanho = 100.dp, cor1 = Color.Yellow, cor3 = Color.Red, padding = 10.dp)
}

1.  Se quisermos permitir que ao usar um componente se possa aplicar *modifiers* sem ser usando argumentos separados (o que se torna problemático porque se quisermos permitir muitos ajustes os argumentos acabarão por ser demasiados) pode-se fazer desta forma em que se aceita que o *modifier* seja fornecido na chamada à função. Note-se que existe uma enorme diferença entre se usar `modifier` (a variável ou argumento que tem o valor que vem de fora) ou `Modifier` (um *modifier vazio*), é muito fácil ter bugs causadas por se usar um M maiúsculo quando se devia ter usado um m minúsculo ou vice-versa.

[![](https://ccti.ismai.pt/and/images/thumb/0/02/Column-with-3boxes-checkbox-with-modifiers-with-args.png/300px-Column-with-3boxes-checkbox-with-modifiers-with-args.png)](https://ccti.ismai.pt/android/File:Column-with-3boxes-checkbox-with-modifiers-with-args.png)

@Composable
fun CirculosQuadradosCheckbox(tamanho: Dp, cor1: Color = Color.Red, cor2: Color = Color.Blue, cor3: Color = Color.Yellow, modifier: Modifier = Modifier) {
   Column() {
       Box(modifier = modifier.fillMaxWidth().size(tamanho, tamanho / 2).background(cor1).clip(CircleShape))
       Box(modifier = modifier.shadow(20.dp, RoundedCornerShape(8.dp)).size(tamanho + 10.dp).background(cor2).clip(CircleShape).background(cor3))
       Row() {
           Box(
               modifier = modifier.clip(CircleShape).background(Color.Black).size(tamanho / 2 + 10.dp)
           )
           Text(text = "Gravação automática", modifier = modifier.align(Alignment.CenterVertically).weight(1f), textAlign = TextAlign.Right)
           Checkbox(checked = false, onCheckedChange = { }, modifier = modifier.align(Alignment.CenterVertically).weight(0.2f))
       }
   }
}
@Preview
@Composable
fun CirculosQuadradosPreview() {
   CirculosQuadradosCheckbox(tamanho = 100.dp, cor1 = Color.Yellow, cor3 = Color.Red, modifier = Modifier.padding(10.dp))
}

1.  `Modifier.verticalScroll(rememberScrollState())` para ser usado como *modifier* de um `Column`
    1.  Assinatura completa da função: `fun Modifier.verticalScroll(state: ScrollState, enabled: Boolean = true, flingBehavior: FlingBehavior? = null, reverseScrolling: Boolean = false ) { ... }`
    2.  `scrollState` determina a distância (*offset*) do topo, e pode também permitir arrancar ou parar *fling animations* (arrastar e depois levantar o dedo rapidamente) ou *smooth scrolling*
    3.  Se `enabled` for false pode-se programaticamente fazer *scroll' para uma dada posição mas o utilizador não pode movimentar o *scroll
    4.  `flingBehavior` é para fazer uma animação com um dado comportamento
    5.  `reverseScroll` por omissão é falso, se for true permite fazer scroll para cima
    6.  Só deve ser usado para uma pequena ou média quantidade de items estáticos, isso porque todos os elementos são antecipadamente calculados o que pode originar uma utilização elevada de CPU se forem muitos itens, nesse caso deve-se usar `LazyColumn`
2.  `Modifier.horizontalScroll(rememberScrollState())` para ser usado como *modifier* de um `Row`
    1.  Assinatura completa da função: `fun Modifier.horizontalScroll(state: ScrollState, enabled: Boolean = true, flingBehavior: FlingBehavior? = null, reverseScrolling: Boolean = false ) { ... }`
    2.  `scrollState` determina a distância (*offset*) do topo, e pode também permitir arrancar ou parar *fling animations* (arrastar e depois levantar o dedo rapidamente) ou *smooth scrolling*
    3.  Se `enabled` for false pode-se programaticamente fazer *scroll' para uma dada posição mas o utilizador não pode movimentar o *scroll
    4.  `flingBehavior` é para fazer uma animação com um dado comportamento
    5.  `reverseScroll` por omissão é falso, se for true permite fazer scroll para cima
    6.  Só deve ser usado para uma pequena ou média quantidade de items estáticos, isso porque todos os elementos são antecipadamente calculados o que pode originar uma utilização elevada de CPU se forem muitos itens, nesse caso deve-se usar `LazyRow`

Recursos
--------

### Adicionar uma imagem

1.  Clicar em `res`
2.  Clicar com o botão da direita em `drawable`
3.  no macOS escolher *Open In / Finder*, em Windows escolher *Show in Explorer*
4.  Duplo click na pasta `drawable`
5.  Copiar para lá o ficheiro com a imagem, e se necessário mudar o nome de modo a ficar um nome que só tenha letras minúsculas (*a-z*), dígitos (*0-9*) ou underscore (*_*), por exemplo `nome_ficheiro.png`
6.  No código Kotlin referenciar a imagem usando `@drawable/nome_ficheiro` (isto é, o nome sem a extensão)

### Adicionar um ícone

1.  No lado esquerdo em qualquer lugar da árvore do projeto clicar com o botão da direita e escolher *New / Vector Asset*
2.  Clicar no lado esquerdo a meio no ícone que aparece à direita de *Clip art:* e pesquisar ou escolher o ícone apropriado
3.  Pode-se mudar o nome desde que se respeite só ter letras minúsculas (a-z), dígitos (0-9) ou underscore (_), , por exemplo `nome_ficheiro.xml`
4.  Premir *Next*
5.  Premir *Finish*
6.  No código Kotlin referenciar a imagem usando `@drawable/nome_ficheiro` (isto é, o nome sem a extensão)
7.  Atenção que o ícone pode ter

### Adicionar uma cor a `colors.xml`

1.  Se ocorrer o erro "*...:color/colorPrimary) not found*", causado por exemplo por `<item android:drawable="@color/colorPrimary" />` num *res/drawable/*.xml* então adicionar a `res/values/colors.xml` algo de semelhante a por exemplo `<color name="colorPrimary">@color/blue_1</color>` seguido de `<color name="blue_1">#00101f</color>`

### Adicionar um string a `strings.xml`

1.  O código do programa não deve incluir textos fixos, deve em vez disso referir *string resources* que são armazenados em `strings.xml`, isto facilita a posterior tradução da App para por exemplo funcionar em português e em inglês
2.  Adicionar por exemplo `<string name="textoCodigo">Texto pretendido</string>`, sendo a seguir possível usar `stringResource(id = R.string.textoCodigo)` para obter a string `"Texto pretendido"`
3.  Note-se que a maneira mais rápida de definir a string é começar por declarar o id, escrevendo por exemplo `stringResource(id = R.string.etiquetaApelido)` e a seguir pairar com o cursor sobre o erro (isto é, pairar sobre `R.string.etiquetaApelido`) e premir **Alt+Shift+Enter** para abrir a janela que permite definir o `New String Value Resource`, desta forma o código já está preenchido e só fica a faltar escrever o texto propriamente dito

Fornecer e receber dados do interface gráfico (gerir o "estado" da App)
-----------------------------------------------------------------------

1.  O utilizador comunica com a App clicando, arrastando, escrevendo, o que despoleta eventos ao nível da App
2.  Os eventos são despoletados por inputs criados fora da App (consequência de ações do utilizador), o "estado" (conjunto de valores armazenados nas variáveis do programa) é o resultado da reação da App ao evento, para se chegar ao "estado" final temos de executar as funções que atualizam o "estado"
3.  O *update loop* consiste em **eventos** que despoletam uma **atualização do estado** que despoleta a **visualização do novo estado**, e assim sucessivamente:
    1.  Evento: input do utilizador ou de outra parte do programa
    2.  Atualizar o estado: *event handler*, reage ao evento atualizando o estado (os dados)
    3.  Mostrar (visualizar) o novo estado: o interface gráfico atualiza a visualização dos dados
4.  No Jetpack compose usa-se *unidirectional data flow*, isto é, o fluxo de dados ocorre num só sentido:
    1.  O interface gráfico reage ao utilizador através do *event handler* que atualiza o *estado* (isto é, usando eventos o fluxo é do input que vem do interface gráfico para o gestor do estado)
    2.  Por sua vez o interface gráfico também observa o estado, cada vez que existe um novo estado o interface gráfico faz a sua visualização (isto é, reagindo a alterações do estado o fluxo é do gestor do estado para atualizar o output no interface gráfico)
5.  O Android oferece dois componentes arquitetónicos de apoio a este fluxo unidirecional dos dados:
    1.  ViewModel: permite *extrair* o estado do interface gráfico e definir eventos que o interface gráfico pode chamar para atualizar o "estado"
    2.  LiveData: permite criar *observable state holders* (armazenadores do estado que podem ser observados) que permitem observar (isto é, detetar) alterações do estado

    O ViewModel representa o "estado", os *composables* representam o interface gráfico, no ViewModel usa-se LiveData para armazenar o "estado"

6.  Para usar o ViewModel adiciona-se aos composables o argumento `viewModel: MainViewModel`
7.  Para navegar entre vários ecrãs da App usa-se:
    1.  No "MainActivity.kt" adiciona-se `val navController = rememberNavController()`, o NavController facilita a navegação entre os diferentes ecrãs da App
    2.  No `SetContent` da MainActivity coloca-se:

   NavHost(navController = navController, startDestination = EcraPrincipal.MyApp.route) {
     composable(EcraPrincipal.MyAppp.route) { ComposablePrincipal(viewModel) }
   }

1.  FIXME

App para conversão de temperaturas Celsius - Farenheit
------------------------------------------------------

Este exemplo simples inclui:

-   A função de topo `ConverterTemperatura()`
-   A função `TextFieldTemperatura(...)` que possui como argumentos um callback e `aTemperatura: MutableState<String>` que permite receber e devolver o valor atual da temperatura
-   A função `ButtonGroupEscalaDeTemperatura(...)` que possui como argumento `selecionado: MutableState<Int>` para receber a informação de qual checkbox está selecionada (armazena o código inteiro do recurso selecionado)
-   A função `RadioButtonTemperatura(...)` que possui como argumentos um callback e `selecionado: Boolean` para receber a informação se esta checkbox está ou não selecionada

Note-se que tratando-se de funções *composable* as funções para poderem ser *puras* (o que é necessário para que funcione bem a otimização das atualizações do interface gráfico em função das interações com o utilizador) não podem armazenar estado, portanto recebem o estado como um argumento e se necessário atualizam o valor armazenado nesse argumento. É o equivalente a eu ter medo de armazenar dados sensíveis, quando me pedem para processar dados sensíveis (quando a minha função é chamada) o que eu faço é pedir a quem me chamou que me forneça um disco com os dados, faço o processamento e quando termino coloco o resultado de novo nesse disco e a seguir devolvo o disco a quem me chamou, desta forma posso *esquecer tudo* e não preciso de armazenar nada. A razão é obviamente diferente, não é medo de processar dados sensíveis mas sim a necessidade de ter a certeza de que se eu fosse chamado de novo com os mesmos dados (darem-me um outro disco em que o conteúdo inicial desse disco era o mesmo que eu tinha recebido anteriormente) então podem otimizar-me e não chegar a chamar-me, basta duplicar o outro disco porque o resultado final seria esse.

#### Imports adicionais

Esta lista inclui os imports que podem ser necessários para além dos já referenciados noutros locais desta página.

import androidx.compose.material3.MaterialTheme
import androidx.compose.ui.res.stringResource
import androidx.compose.material3.RadioButton
import androidx.compose.runtime.MutableState
import androidx.compose.runtime.mutableStateOf
import androidx.compose.runtime.remember
import androidx.compose.foundation.text.KeyboardOptions
import androidx.compose.foundation.text.KeyboardActions
import androidx.compose.ui.text.input.KeyboardType
import androidx.compose.ui.text.input.ImeAction

#### ConverterTemperatura()

Esta função não possui argumentos e usa 3 variáveis do tipo `remember(mutableStableOf(...))` e uma variável do tipo `remember(...)` para armazenar o seguinte:

-   `campoTemperatura`:
-   `campoEscala`:
-   `temperaturaConvertida`:
-   `resultado`:

Note-se que se rodarmos o telemóvel/emulador de retrato para paisagem ou vice-versa perde-se o valor atual de todas estas variáveis, isso porque o interface gráfico é recriado pelo que a função `ConverterTemperatura()` é chamada de novo com a consequência de todas as variáveis serem reinicializadas.

@Composable
@Preview
fun ConverterTemperatura() {
   val strCelsius = stringResource(id = R.string.celsius) // string definido em strings.xml com a palavra "Celsius"
   val strFahrenheit = stringResource(id = R.string.fahrenheit) // string definido em strings.xml com a palavra "Farenheit"
   val campoTemperatura = remember { mutableStateOf("") } // string que representa uma temperatura pelo que ou está vazio ou tem dígitos (número com casas decimais)
   val campoEscala = remember { mutableStateOf(R.string.celsius) } // inteiro que me diz qual dos radio buttons está selecionado
   var temperaturaConvertida = remember { mutableStateOf(Float.NaN) } // temperatura já convertida para um float ou o valor NaN (not a number)
   val calcular = {  // lambda guardado numa variável de modo a poder ser utilizado em 2 sítios diferentes (no TextField e no Button)
       val temp = campoTemperatura.value.toFloat()
       temperaturaConvertida.value = if (campoEscala.value == R.string.celsius) (temp * 1.8F) + 32F else (temp - 32F) / 1.8F
   }
   val resultado = remember(temperaturaConvertida.value) {
       if (temperaturaConvertida.value.isNaN()) ""
       else
           "${temperaturaConvertida.value} ${
               if (campoEscala.value == R.string.celsius)
                   strFahrenheit
               else strCelsius
           }"
   }
   val ativado = campoTemperatura.value.isNotBlank()
   Column(modifier = Modifier.fillMaxSize().padding(16.dp), horizontalAlignment = Alignment.CenterHorizontally) {
       TextFieldTemperatura(aTemperatura = campoTemperatura, modifier = Modifier.padding(bottom = 16.dp), callback = calcular)
       ButtonGroupEscalaDeTemperatura(selecionado = campoEscala, modifier = Modifier.padding(bottom = 16.dp))
       Button(onClick = calcular, enabled = ativado) {
           Text(text = stringResource(id = R.string.convert))
       }
       if (resultado.isNotEmpty()) {
           Text(text = resultado, style = MaterialTheme.typography.headlineMedium)
       }
   }
}

e eis outra solução, mais simples, neste caso optou-se por não manter atualizado o float da temperatura e só o calcular quando se carrega no botão, por isso um dos lambdas passou a estar vazio, note-se o uso de `resultado.value` em vários sítios (ver [como usar mutable state](https://ccti.ismai.pt/android/Jetpack_Compose#remember_e_mutableStateOf), é um erro muito comum usar `resultado` quando se devia estar a usar `resultado.value`):

@Composable
@Preview
fun ConverterTemperatura() {
   val campoTemperatura = remember { mutableStateOf("") } // string que representa uma temperatura pelo que ou está vazio ou tem dígitos (número com casas decimais)
   val campoEscala = remember { mutableStateOf(R.string.celsius) } // inteiro que me diz qual dos radio buttons está selecionado
   var resultado = remember { mutableStateOf("") }
   val calcular = {
       val temperatura = campoTemperatura.value.toFloat()
       val r: Float
       if (campoEscala.value == R.string.celsius)
           r = temperatura * 9 / 5 + 32
       else
           r = (temperatura - 32) * 5 / 9
       resultado.value = r.toString()
   }
   val ativado = campoTemperatura.value.isNotBlank()
   Column(modifier = Modifier
       .fillMaxSize()
       .padding(16.dp), horizontalAlignment = Alignment.CenterHorizontally) {
       TextFieldTemperatura(aTemperatura = campoTemperatura, modifier = Modifier.padding(bottom = 16.dp), callback = { } )
       ButtonGroupEscalaDeTemperatura(selecionado = campoEscala, modifier = Modifier.padding(bottom = 16.dp))
       Button(onClick = calcular, enabled = ativado) {
           Text(text = stringResource(id = R.string.convert))
       }
       if (resultado.value.isNotEmpty()) {
           Text(text = resultado.value, style = MaterialTheme.typography.headlineMedium)
       }
   }
}

#### TextFieldTemperatura(aTemperatura: MutableState<String>, modifier: Modifier = Modifier, callback: () -> Unit)

A função `TextFieldTemperatura(...)` possui como argumentos, nesta ordem:

-   `aTemperatura`: um string que serve para receber a informação da temperatura atual e para além disso serve para atualizar (isto é, passar para a função que chamou esta) esse valor, desta forma esta função consegue atualizar o estado da aplicação ao mesmo tempo que se mantém pura
-   `callback`: um callback (um *lambda*) que diz o que fazer quando no teclado se clica no símbolo do *done*
-   `modifier`: para ajustes gráficos, por omissão é inicializado com um modifier vazio e neste caso é passado ao `TextField`

internamente usa-se `onValueChange` para se atualizar o valor do argumento `aTemperatura` sempre que o utilizador introduz um carater, optou-se por se usar um *placeholder* para ajudar o utilizador a saber o que fazer (help text), e usou-se o argumento `keyboardActions` do `TextField` para se forçar a que no teclado só se possa introduzir números (desta forma evita-se que a aplicação faça *crash* se alguém escrever texto), e define-se o que se pretende que apareça no teclado como símbolo de que a operação de introdução do valor está concluída, neste caso não é obrigatório que o utilizador clique nesse símbolo, em alternativa o utilizador pode usar o botão definido na função que chama esta, isso porque o `onCLick` do botão manda executar o mesmo lambda (guardado na variável `calcular` de modo ao mesmo código poder ser usado em 2 sítios diferentes).

@Composable
fun TextFieldTemperatura(aTemperatura: MutableState<String>, callback: () -> Unit, modifier: Modifier = Modifier) {
   TextField(value = aTemperatura.value, onValueChange = { aTemperatura.value = it },
       placeholder = { Text(text = stringResource(id = R.string.placeholder)) },
       modifier = modifier,
       keyboardActions = KeyboardActions(onAny = { callback() }),
       keyboardOptions = KeyboardOptions(keyboardType = KeyboardType.Number, imeAction = ImeAction.Done),
       singleLine = true
   )
}

#### ButtonGroupEscalaDeTemperatura(selecionado: MutableState<Int>, modifier: Modifier = Modifier)

A função `ButtonGroupEscalaDeTemperatura(...)` possui como argumentos, nesta ordem:

-   `selecionado` um inteiro que serve para receber a informação de qual checkbox está selecionada e para além disso serve para atualizar (isto é, passar para a função que chamou esta) esse valor, desta forma esta função consegue atualizar o *estado* da aplicação ao mesmo tempo que se mantém *pura*
-   `modifier`: para ajustes gráficos, por omissão é inicializado com um *modifier* vazio e neste caso só é passado ao `Row`

@Composable
fun ButtonGroupEscalaDeTemperatura(selecionado: MutableState<Int>, modifier: Modifier = Modifier) {
   val sel = selecionado.value
   val onClick = { resId: Int -> selecionado.value = resId }
   Row(modifier = modifier) {
       RadioButtonTemperatura(selecionado = sel == R.string.celsius, resId = R.string.celsius, onClick = onClick)
       RadioButtonTemperatura(selecionado = sel == R.string.fahrenheit, resId = R.string.fahrenheit, onClick = onClick, modifier = Modifier.padding(start = 16.dp))
   }
}

#### RadioButtonTemperatura(selecionado: Boolean, resId: Int, onClick: (Int) -> Unit, modifier: Modifier = Modifier)

A função `RadioButtonTemperatura(...)` possui como argumentos, nesta ordem:

-   `selecionado` um booleano que serve para receber a informação se esta checkbox está ou não selecionada
-   `resId`: um inteiro que identifica o recurso (uma string) que contém o texto que deve aparecer ao lado do radio button
-   Um callback que contém o código que deve ser executado quando alguém clica neste *radio button*
-   `modifier`: para ajustes gráficos, por omissão é inicializado com um *modifier* vazio e neste caso só é passado ao `Row`

@Composable
fun RadioButtonTemperatura(selecionado: Boolean, resId: Int, onClick: (Int) -> Unit, modifier: Modifier = Modifier) {
   Row(verticalAlignment = Alignment.CenterVertically, modifier = modifier) {
       RadioButton(selected = selecionado, onClick = { onClick(resId) })
       Text(text = stringResource(resId), modifier = Modifier.padding(start = 8.dp))
   }
}

### Scratch

package pt.umaia.cm2024.myappone

import android.os.Bundle
import androidx.activity.ComponentActivity
import androidx.activity.compose.setContent
import androidx.activity.enableEdgeToEdge
import androidx.compose.foundation.layout.Column
import androidx.compose.foundation.layout.Row
import androidx.compose.foundation.layout.fillMaxSize
import androidx.compose.foundation.layout.padding
import androidx.compose.foundation.text.KeyboardActions
import androidx.compose.foundation.text.KeyboardOptions
import androidx.compose.material3.Button
import androidx.compose.material3.MaterialTheme
import androidx.compose.material3.RadioButton
import androidx.compose.material3.Scaffold
import androidx.compose.material3.Text
import androidx.compose.material3.TextField
import androidx.compose.runtime.Composable
import androidx.compose.runtime.MutableState
import androidx.compose.runtime.mutableStateOf
import androidx.compose.runtime.remember
import androidx.compose.ui.Alignment
import androidx.compose.ui.Modifier
import androidx.compose.ui.res.stringResource
import androidx.compose.ui.text.input.ImeAction
import androidx.compose.ui.text.input.KeyboardType
import androidx.compose.ui.tooling.preview.Preview
import androidx.compose.ui.unit.dp
import pt.umaia.cm2024.myappone.ui.theme.MyAppOneTheme

class MainActivity : ComponentActivity() {
   override fun onCreate(savedInstanceState: Bundle?) {
       super.onCreate(savedInstanceState)
       enableEdgeToEdge()
       setContent {
           MyAppOneTheme {
               Scaffold(modifier = Modifier.fillMaxSize()) { innerPadding ->
                   ConverterTemperatura(
                       modifier = Modifier.padding(innerPadding)
                   )
               }
           }
       }
   }
}

@Composable
fun ConverterTemperatura(modifier: Modifier) {
   val campoTemperatura = remember { mutableStateOf("") } // string que representa uma temperatura pelo que ou está vazio ou tem dígitos (número com casas decimais)
   val campoEscala = remember { mutableStateOf(R.string.celsius) } // inteiro que me diz qual dos radio buttons está selecionado
   var resultado = remember { mutableStateOf("") }
   val calcular = {
       val temperatura = campoTemperatura.value.toFloat()
       val r: Float
       if (campoEscala.value == R.string.celsius)
           r = temperatura * 9 / 5 + 32
       else
           r = (temperatura - 32) * 5 / 9
       resultado.value = r.toString()
   }
   val ativado = campoTemperatura.value.isNotBlank()
   Column(modifier = Modifier
       .fillMaxSize()
       .padding(16.dp), horizontalAlignment = Alignment.CenterHorizontally) {
       TextFieldTemperatura(aTemperatura = campoTemperatura, modifier = Modifier.padding(bottom = 16.dp), callback = { } )
       ButtonGroupOpcoes(selecionado = campoEscala, modifier = Modifier.padding(bottom = 16.dp))
       Button(onClick = calcular, enabled = ativado) {
           Text(text = stringResource(id = R.string.convert))
       }

       if (resultado.value.isNotEmpty()) {
           Text(text = resultado.value, style = MaterialTheme.typography.headlineMedium)
       }
   }
}

@Composable
fun TextFieldTemperatura(aTemperatura: MutableState<String>, callback: () -> Unit, modifier: Modifier = Modifier) {
   TextField(value = aTemperatura.value, onValueChange = { aTemperatura.value = it },
       placeholder = { Text(text = stringResource(id = R.string.placeholder)) },
       modifier = modifier,
       keyboardActions = KeyboardActions(onAny = { callback() }),
       keyboardOptions = KeyboardOptions(keyboardType = KeyboardType.Number, imeAction = ImeAction.Done),
       singleLine = true
   )
}
@Composable
fun ButtonGroupOpcoes(selecionado: MutableState<Int>, modifier: Modifier = Modifier) {
   val sel = selecionado.value
   val onClick = { resId: Int -> selecionado.value = resId }
   Column(modifier = modifier) {
       MeuRadioButton(selecionado = sel == R.string.evento, resId = R.string.evento, onClick = onClick)
       MeuRadioButton(selecionado = sel == R.string.artigo, resId = R.string.artigo, onClick = onClick, modifier = Modifier.padding(start = 16.dp))
       MeuRadioButton(selecionado = sel == R.string.projeto, resId = R.string.projeto, onClick = onClick, modifier = Modifier.padding(start = 16.dp))
   }
}
@Composable
fun MeuRadioButton(selecionado: Boolean, resId: Int, onClick: (Int) -> Unit, modifier: Modifier = Modifier) {
   Row(verticalAlignment = Alignment.CenterVertically, modifier = modifier) {
       RadioButton(selected = selecionado, onClick = { onClick(resId) })
       Text(text = stringResource(resId), modifier = Modifier.padding(start = 8.dp))
   }
}

Criar uma App com 4 ecrãs
-------------------------

Antes de começar é necessário colocar no *build.gradle* do **módulo** dentro da secção `dependencies { ...}` estas 2 bibliotecas:

-   `val nav_version = "2.8.2"`
-   `implementation("androidx.navigation:navigation-compose:$nav_version")`
-   `val compose_material_version = "1.7.3"`
-   `implementation("androidx.compose.material:material:$compose_material_version")` // necessário para se poder usar a *BottomNavigation*

(a seguir não esquecer de fazer o *sync*)

Optou-se por organizar o código em 3 ficheiros:

-   Ecras.kt com o interface gráfico dos 4 ecrãs propriamente ditos
-   Destinos.kt para definir os ícones e os objetos relacionados com o *routing* (navegação) entre os ecrãs
-   MainActivity.kt com o programa principal que utiliza um *Scaffold* e uma Bottom Navigation Bar para criar uma App com 4 ecrãs

Para criar cada um dos 2 ficheiros usar: "right click no MainActivity.kt / New / Kotlin Class/File / File (e colocar o nome)"

NOTAS:

1.  Embora esta aplicação só mostre texto em cada um dos 4 ecrãs basta substituir o conteúdo da função correspondente ao *compose* de cada ecrã por algo apropriado para se ter uma aplicação que funcione
2.  E como é que se partilha o valor das variáveis entre mais do que um ecrã? Basta, por exemplo, fazer com que o `var campo1 = remember { mutableStateOf("") }` em vez de ser declarado no topo do ecrã 1 seja declarado a um nível superior (neste caso na função `ProgramaPrincipal`), e que na função `AppNavigation` se adicione um argumento para receber o campo e em vez de se chamar `Ecra01()` e `Ecra02()` se chame `Ecra01(campo1)` e `Ecra02(campo1)`, e que em `ecras.kt` se altere de `fun Ecra01() {...}` e `fun Ecra02() {...}` para `fun Ecra01(oCampo: MutableState<String>) {...}` e `fun Ecra02(oCampo: MutableState<String>) {...}` para que se consiga partilhar variáveis entre mais do que um ecrã (isto é, alterar no ecrã 1 o argumento `oCampo` faz com que o novo valor apareça no argumento `oCampo` do ecrã 2 visto que existe um `remember` no nível superior da variável `campo1` que está a ser partilhada entre os 2 ecrãs ao ser passada como argumento a ambos os ecrãs). Note-se que se existir uma alteração da configuração do ecrã (por exemplo rodar de forma a passar de *retrato/portrait* para *paisagem/landscape*) os dados são perdidos se se estiver a usar `var campo1 = remember { mutableStateOf("") }`, para que os dados não sejam perdidos tem de se usar `var campo1 = rememberSaveable { mutableStateOf("") }`

### Ecras.kt

package pt.ismai.ccti2023.navegar

import androidx.compose.foundation.layout.Column
import androidx.compose.foundation.layout.fillMaxSize
import androidx.compose.foundation.layout.wrapContentSize
import androidx.compose.material3.Text
import androidx.compose.runtime.Composable
import androidx.compose.ui.Alignment
import androidx.compose.ui.Modifier
import androidx.compose.ui.graphics.Color
import androidx.compose.ui.res.stringResource
import androidx.compose.ui.text.font.FontWeight
import androidx.compose.ui.text.style.TextAlign
import androidx.compose.ui.unit.sp

@Composable
fun Ecra01() {
   Column(modifier = Modifier.fillMaxSize().wrapContentSize(Alignment.Center)) {
       Text(text = stringResource(id = R.string.ecra01),
           fontWeight = FontWeight.Bold, color = Color.Gray,
           modifier = Modifier.align(Alignment.CenterHorizontally),
           textAlign = TextAlign.Center, fontSize = 18.sp
       )
   }
}

@Composable
fun Ecra02() {
   Column(modifier = Modifier.fillMaxSize().wrapContentSize(Alignment.Center)) {
       Text(text = stringResource(id = R.string.ecra02),
           fontWeight = FontWeight.Bold, color = Color.Gray,
           modifier = Modifier.align(Alignment.CenterHorizontally),
           textAlign = TextAlign.Center, fontSize = 18.sp
       )
   }
}

@Composable
fun Ecra03() {
   Column(modifier = Modifier.fillMaxSize().wrapContentSize(Alignment.Center)) {
       Text(text = stringResource(id = R.string.ecra03),
           fontWeight = FontWeight.Bold, color = Color.Gray,
           modifier = Modifier.align(Alignment.CenterHorizontally),
           textAlign = TextAlign.Center, fontSize = 18.sp
       )
   }
}

@Composable
fun Ecra04() {
   Column(modifier = Modifier.fillMaxSize().wrapContentSize(Alignment.Center)) {
       Text(text = stringResource(id = R.string.ecra04),
           fontWeight = FontWeight.Bold, color = Color.Gray,
           modifier = Modifier.align(Alignment.CenterHorizontally),
           textAlign = TextAlign.Center, fontSize = 18.sp
       )
   }
}

### Destinos.kt

A classe foi marcada *selada* de modo a não ser possível estendê-la herdando dela (isso não é obrigatório fazer mas representa o facto de que não queremos que apareçam mais ecrãs definidos noutro lado). Os ícones tem de ser adicionados um a um recorrendo ao 'clipart* do Android: (clicar com o botão da direita sobre "res") New / Vector Asset / na terceira linha onde diz "Clip art:" clicar no ícone para aparecer a janela com a clipart / usando a pesquisa escolher um ícone / premir OK / Next / Finish.*

Note-se que não é obrigatório aceitar o nome do *clipart*, por exemplo em baixo, ao selecionar o clipart antes de se premir OK poderia ter-se alterado o nome de `baseline_add_shopping_cart_24` para `carrinho_compras`, se isso tivesse sido feito então teriamos de usar `R.drawable.carrinho_compras` (atenção que os nomes tem de ser todos com letras minúsculas e opcionalmente digitos e underscores).

package pt.ismai.ccti2023.navegar

sealed class Destino(val route: String, val icon: Int, val title: String) {
   object Ecra01 : Destino(route = "ecra01", icon = R.drawable.baseline_add_shopping_cart_24, title = "Ecra01")
   object Ecra02 : Destino(route = "ecra02", icon = R.drawable.baseline_access_alarm_24, title = "Ecra02")
   object Ecra03 : Destino(route = "ecra03", icon = R.drawable.baseline_archive_24, title = "Ecra03")
   object Ecra04 : Destino(route = "ecra04", icon = R.drawable.baseline_app_settings_alt_24, title = "Ecra04")
   companion object {
       val toList = listOf(Ecra01, Ecra02, Ecra03, Ecra04)
   }
}

### MainActivity.kt

Sugere-se a adição incial destes *imports* já que é fácil selecionar o import errado:

package pt.ismai.ccti2023.navegar
import pt.ismai.ccti2023.navegar.ui.theme.MyApplicationTheme

import android.os.Bundle
import androidx.activity.ComponentActivity
import androidx.activity.compose.setContent
import androidx.compose.foundation.layout.Box
import androidx.compose.foundation.layout.fillMaxSize
import androidx.compose.foundation.layout.padding
import androidx.compose.material.BottomNavigation
import androidx.compose.material.BottomNavigationItem
import androidx.compose.material3.ExperimentalMaterial3Api
import androidx.compose.material3.Icon
import androidx.compose.material3.MaterialTheme
import androidx.compose.material3.Scaffold
import androidx.compose.material3.Surface
import androidx.compose.material3.Text
import androidx.compose.runtime.Composable
import androidx.compose.runtime.getValue
import androidx.compose.ui.Modifier
import androidx.compose.ui.graphics.Color
import androidx.compose.ui.res.colorResource
import androidx.compose.ui.res.painterResource
import androidx.compose.ui.tooling.preview.Preview
import androidx.navigation.NavController
import androidx.navigation.NavHostController
import androidx.navigation.compose.NavHost
import androidx.navigation.compose.composable
import androidx.navigation.compose.currentBackStackEntryAsState
import androidx.navigation.compose.rememberNavController

Atenção que o tema (`MyApplicationTheme`) tem de ser adaptado para o que estiver a ser usado na aplicação. Se a barra de navegação inferior não aparecer experimentar na classe MainActivity comentar a instrução `enableEdgeToEdge()`, ver a documentação de [edge-to-edge](https://developer.android.com/develop/ui/views/layout/edge-to-edge)

class MainActivity : ComponentActivity() {
   override fun onCreate(savedInstanceState: Bundle?) {
       super.onCreate(savedInstanceState)
       setContent {
           MyApplicationTheme {
               Surface(modifier = Modifier.fillMaxSize(), color = MaterialTheme.colorScheme.background) {
                   ProgramaPrincipal()
               }
           }
       }
   }
}

// Programa principal que utiliza o `Scaffold` para suportar uma barra de navegação no fundo do ecrã que permite navegar para cada um dos 4 ecrãs.

@Composable
fun ProgramaPrincipal() {
   val navController = rememberNavController()
   Scaffold(
       bottomBar = { BottomNavigationBar(navController = navController, appItems = Destino.toList) },
       content = { padding ->
           Box(modifier = Modifier.padding(padding)) {
               AppNavigation(navController = navController)
           }
       }
   )
}

// Função para permitir navegar para o ecrã pretendido de entre os 4 ecrãs, neste caso optou-se por usar o "Ecra01" como ecrã de arranque (`startDestination`)

@Composable
fun AppNavigation(navController: NavHostController) {
  NavHost(navController, startDestination = Destino.Ecra01.route) {
      composable(Destino.Ecra01.route) {
          Ecra01()
      }
      composable(Destino.Ecra02.route) {
          Ecra02()
      }
      composable(Destino.Ecra03.route) {
          Ecra03()
      }
      composable(Destino.Ecra04.route) {
          Ecra04()
      }
  }
}

// Função para gerir a barra de navegação no fundo do ecrã (completamente reutilizável exceto assumir a existência da classe `Destino`).

@Composable
fun BottomNavigationBar(navController: NavController, appItems: List<Destino>) {
   BottomNavigation(backgroundColor = colorResource(id = R.color.purple_700),contentColor = Color.White) {
       val navBackStackEntry by navController.currentBackStackEntryAsState()
       val currentRoute = navBackStackEntry?.destination?.route
       appItems.forEach { item ->
           BottomNavigationItem(
               icon = { Icon(painterResource(id = item.icon), contentDescription = item.title, tint=if(currentRoute == item.route) Color.White else Color.White.copy(.4F)) },
               label = { Text(text = item.title, color = if(currentRoute == item.route) Color.White else Color.White.copy(.4F)) },
               selectedContentColor = Color.White, // esta instrução devia funcionar para o efeito (animação), para o ícone e para a cor do texto, mas só funciona para o efeito
               unselectedContentColor = Color.White.copy(0.4f), // esta instrução não funciona, por isso resolve-se acima no 'tint' do icon e na 'color' da label
               alwaysShowLabel = true, // colocar 'false' significa que o texto só aparece debaixo do ícone selecionado (em vez de debaixo de todos)
               selected = currentRoute == item.route,
               onClick = {
                   navController.navigate(item.route) {
                       navController.graph.startDestinationRoute?.let { route -> popUpTo(route) { saveState = true } }
                       launchSingleTop = true
                       restoreState = true
                   }
               }
           )
       }
   }
}

<-- [Voltar à página hierarquicamente anterior](https://ccti.ismai.pt/android/Main_Page "Main Page")

Navigation menu
---------------

-   [Log in](https://ccti.ismai.pt/and/index.php?title=Special:UserLogin&returnto=Jetpack+Compose "You are encouraged to log in; however, it is not mandatory [alt-shift-o]")

-   [Page](https://ccti.ismai.pt/android/Jetpack_Compose "View the content page [alt-shift-c]")
-   [Discussion](https://ccti.ismai.pt/and/index.php?title=Talk:Jetpack_Compose&action=edit&redlink=1 "Discussion about the content page (page does not exist) [alt-shift-t]")

-   [Read](https://ccti.ismai.pt/android/Jetpack_Compose)
-   [View source](https://ccti.ismai.pt/and/index.php?title=Jetpack_Compose&action=edit "This page is protected.
    You can view its source [alt-shift-e]")
-   [View history](https://ccti.ismai.pt/and/index.php?title=Jetpack_Compose&action=history "Past revisions of this page [alt-shift-h]")

### Search

[](https://ccti.ismai.pt/android/Main_Page "Visit the main page")

-   [Main page](https://ccti.ismai.pt/android/Main_Page "Visit the main page [alt-shift-z]")
-   [Recent changes](https://ccti.ismai.pt/android/Special:RecentChanges "A list of recent changes in the wiki [alt-shift-r]")
-   [Random page](https://ccti.ismai.pt/android/Special:Random "Load a random page [alt-shift-x]")
-   [Help about MediaWiki](https://www.mediawiki.org/wiki/Special:MyLanguage/Help:Contents)

### Tools

-   [What links here](https://ccti.ismai.pt/android/Special:WhatLinksHere/Jetpack_Compose "A list of all wiki pages that link here [alt-shift-j]")
-   [Related changes](https://ccti.ismai.pt/android/Special:RecentChangesLinked/Jetpack_Compose "Recent changes in pages linked from this page [alt-shift-k]")
-   [Special pages](https://ccti.ismai.pt/android/Special:SpecialPages "A list of all special pages [alt-shift-q]")
-   Printable version
-   [Permanent link](https://ccti.ismai.pt/and/index.php?title=Jetpack_Compose&oldid=1041 "Permanent link to this revision of this page")
-   [Page information](https://ccti.ismai.pt/and/index.php?title=Jetpack_Compose&action=info "More information about this page")
-   [Cite this page](https://ccti.ismai.pt/and/index.php?title=Special:CiteThisPage&page=Jetpack_Compose&id=1041&wpFormIdentifier=titleform "Information on how to cite this page")

-   This page was last modified on 14 October 2024, at 12:08.
-   Content is available under [Creative Commons Attribution-NonCommercial-ShareAlike](https://creativecommons.org/licenses/by-nc-sa/4.0/) unless otherwise noted.

-   [Privacy policy](https://ccti.ismai.pt/android/ANDROID:Privacy_policy)
-   [About ANDROID](https://ccti.ismai.pt/android/ANDROID:About)
-   [Disclaimers](https://ccti.ismai.pt/android/ANDROID:General_disclaimer)

-   [![Creative Commons Attribution-NonCommercial-ShareAlike](https://ccti.ismai.pt/and/resources/assets/licenses/cc-by-nc-sa.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
-   [![Powered by MediaWiki](https://ccti.ismai.pt/and/resources/assets/poweredby_mediawiki_88x31.png)](https://www.mediawiki.org/)
