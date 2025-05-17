# 🤠 Projeto Chico Bento – Seu Amigo Caipira nas Compras!

<p align="center">
  <img src="IMAGEM DO CHICO.PNG" alt="Imagem do Chico Bento" width="300">
  
  <br>
</p>

E aí, cumpadi e cumadi! Já se sentiu mais perdido que cego em tiroteio nas prateleira do mercado? Nóis sabe como é! Fila grande, tempo curto, e cadê aquele produto que a gente precisa? Eita, aperreio! 😫

É pra mode ajudá nessas horas que nasceu o **Chico Bento**, um assistente virtual com jeitinho da roça, pronto pra te orientá e fazê suas compra ficá mais fácil que tirá doce de criança! 🍬

## 🌽 O Aperreio de Fazê Compra:

* Você tá lá no mercado, aquele mundaréu de gente, e precisa achá um trem específico... mas num tem uma viva alma do mercado pra te socorrê. Triste, né não? 😥

* Ou intão, tá atrasado pro trabaio e só precisa pegá uma pasta de dente rapidinho. Onde será que fica? 🏃‍♂️💨

* E quando dá aquela vontade de um biscoito integral? Tem tanta marca... Qual levá? O mais barato? O mais gostoso? Um de cada pra num errá? É dúvida que não acaba mais! 🍪🤔

## ✨ A Ajuda do Chico Bento:

Imagina só: você chega no mercado e dá de cara com o Chico Bento, prontinho pra te atendê num painel digital ou direto no seu celular! Com dois dedo de prosa, ele te ajuda:

* **Achar os produto:** "Chico, onde é que tá o fubá pra polenta?" E ele te explica o caminho direitinho! 🗺️

* **Saber mais sobre os item:** "Chico, esse detergente aqui é bão mesmo? Tira gordura que é uma beleza?" Ele busca informação pra você! 🧼

* **Comparar as marca e preço:** "Chico, qual marca de biscoito integral tá valendo mais a pena hoje?" Ele te mostra as opção, as avaliação e os preço! (Lembrando que, pra ter os preço atualizadinho e as marca certinha do estoque, o sistema do Chico precisa tá ligado direto no sistema da loja, tá bom?) 📊💰

* **Anotar o que falta:** Se algo num tiver, ele já bota na lista de "mercadoria em farta" pra reposição. 📝

## ⚙️ Pra Botar o Chico pra Funcionar, Vosmecê Vai Precisar de:

Este projeto usa um código Python pra fazer o Chico Bento funcionar. Pra ele prosear direitinho e te ajudar, tem uns segredinhos:

1. **O Código do Chico (`.py`):** É o arquivo principal com toda a inteligência dele. É esse que tá aqui no GitHub!

2. **Um "Caderninho de Anotação" (Planilha Google Sheets):** O Chico guarda as informações dos produtos (nome, preço, onde tá, nota do povo, quantidade) numa planilha do Google Sheets. Sem ela, ele não sabe o que tem no armazém!

   * **Como pegar o "Número de Identidade" (ID) da sua Planilha:**

     1. Abra sua planilha no Google Sheets.

     2. Olhe lá em riba, na barra de endereço do seu navegador. O endereço vai ser comprido, mas no meio dele tem uma parte assim:
        `.../spreadsheets/d/`**`AQUI_FICA_O_ID_DA_SUA_PLANILHA`**`/edit...`
        *Exemplo de ID:* `18ifJ-jluweYUY_1MwYtsNqbApABwo3kwsuOp21OcYa0` (o seu vai ser diferente!)

     3. Copie esse monte de letra e número! É ele que vosmecê vai colocar no código Python do Chico, naquela variável `spreadsheet_id`.

   * **Exemplo de Planilha pra Teste:** Se quiser ver como o Chico organiza o caderninho dele, pode usar uma planilha parecida com essa pra seus testes (lembre de criar a sua própria e usar o ID dela no código):

     | **Nome** | **Descrição** | **Marca** | **Preço** | **Quantidade** | **Nota** | **Localização** | 
     | :------------------ | :-------------------------------------------------------- | :--------------- | :------ | :--------- | :--- | :---------- |
     | Café Torrado | Produto fresquinho, saído da roça direto pro seu lar. | Viver Bem | R$ 5,19 | 1 | 3,3 | E1 | 
     | Leite Integral | Serve tanto pra café da manhã quanto pro almoço. | Casa Caipira | R$10,89 | 3 | 3,5 | A9 | 
     | Biscoito de Polvilho | Receita da vovó fica mió com esse aqui! | Casa Caipira | R$ 5,59 | 5 | 3,2 | C3 | 
     | Farinha de Mandioca | Baratim e muito útil, todo mundo leva. | Rancho Mineiro | R$16,79 | 7 | 4,7 | F13 | 
     | Pão de Forma | Ajuda que só, num pode faltá na dispensa! | Roça Feliz | R$ 9,38 | 91 | 4,9 | E12 | 

3. **A "Chave da Sabedoria Artifiçá" (API Key do Google Gemini):** Pra entender suas perguntas e te dar umas respostas bem caprichadas, o Chico usa a inteligência do Google Gemini. Pra isso, ele precisa de uma "chave" especial, que é a API Key.

   * Vosmê precisa criar essa chave lá no [Google AI Studio](https://aistudio.google.com/app/apikey) (antigo MakerSuite).

   * No ambiente que for rodar o código (como o Google Colab), essa chave precisa ser configurada (por exemplo, como um "Secret" chamado `GOOGLE_API_KEY`).

4. **Um Lugar pra Rodar o Código (Ambiente de Execução):**

   * O **Google Colab** é um lugar bão demais pra rodar o código do Chico! É de graça e já vem com muita coisa pronta. O código foi feito pensando nele.

   * Se for rodar no seu computador, vai precisar ter o Python instalado e as bibliotecas que o Chico usa (`gspread`, `pandas`, `google-generativeai`). O código já tem umas linha no começo pra ajudar a instalar isso, se precisar.

## 💬 Como Proseá mais o Chico:

É fácil que nem comê pamonha!

1. Abra o código do Chico no Google Colab (ou no seu ambiente Python).

2. Configure o ID da sua planilha e sua API Key do Gemini no código.

3. Rode o código!

4. O Chico vai te dar um "Olá" e aí é só começar a conversa digitando o que você precisa no campo que aparecer.

5. Ele te responde na hora, com aquele sotaque caprichado!

## 🗣️ Um Dedinho de Prosa com o Chico (Exemplo de Conversa):

**Vosmecê:** *"Olha só, lançaro o Chico Bento, um assistente aqui no mercado! Deixa eu ver como é que funciona esse trem..."*
**Vosmecê:** *"Hum... acho que é só apertá aqui pra 'Começá Prosa'."*

**Chico Bento:** *"Olá, cumpadi, olá, cumadi! Sou o Chico Bento, seu mió assistente nas hora das compra! Em que posso ajudá vosmecês hoje? É só escrevê o que precisa que eu dou um jeito de orientá!"*

**Vosmecê:** *"Chico, preciso sabê onde tão os biscoito integral. Queria um que fosse bão e num muito caro. Qual vosmecê me indica?"*

**Chico Bento:** *"Aguenta as ponta aí, cumpadi! Deixa eu bicuiá aqui rapidinho pra vosmecê... Só um instantinho!"*

**(Depois da busca...)**

**Chico Bento:** *"Óia só! Os biscoito integral tão lá na 🤠 **Seção A1**. É só levantá os óio e procurá as placa no teto com as letra, e nas prateleira tem os número. Num tem erro, é facinho, facinho!"*

**Chico Bento:** *"Das marca que tem aqui hoje, o povo anda falando bem da 👍 **Marca X** (tem avaliação de 5 estrela!) e da 👍 **Marca Z** (com 4 estrela). Parecem que são boa mesmo!"*

**Chico Bento:** *"E o preço tá camarada, viu? A 💰 **Marca X** tá saindo por R$ 5,99 o pacote, e a 💰 **Marca Z** tá R$ 2,59. A Marca X é a que mais sai, mas a Z também tem seu valor!"*

**Chico Bento:** *"Precisa de mais alguma coisa, cumpadi? 🤔 Tô aqui às ordem!"*

**Vosmecê:** *"Era só isso mesmo, Chico! Brigadão pela ajuda, viu? Tenha um bão dia!"*

**Chico Bento:** *"De nada, cumpadi! Fico felizão de ajudá e amo ser seu assistente aqui. Vorta sempre que precisá, viu?! Inté mais ver! 👋"*


## Veja uma prévia do Projeto Chico Bento!
* Você pode baixar ao vídeo do projeto [clicando aqui](Projeto_Chico_Bento.mp4).


Este projeto une a tecnologia com a simpatia e simplicidade do campo, tornando a experiência de compra mais agradável e eficiente para todos! Espero que goste!

Att,

Matheus Tavares 🤠
