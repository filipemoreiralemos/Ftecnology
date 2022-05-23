

Como fazer um input text aceitar somente números


Caso você ainda deseje um input do tipo texto, veja este snippet:


1- input type="text" oninput="this.value = this.value.replace(/[^0-9.]/g, '').replace(/(\..*?)\..*/g, '$1');" /> 



Ele cria um input de texto, que automaticamente filtra o que foi digitado, não aceitando números

Note que utilizamos um código JavaScript com expressão regular, no atributo oninput
