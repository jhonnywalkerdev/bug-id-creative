# Correção falha de segurança GRAVE ID Login
Corrige uma falha de segurança em bases Creative, que consiste em logar com um outro `user_id` que não pertence a você. Bug presente na maioria das bases Creative.

Basicamente fiz uma verificação, que cria uma condição de checkagem da `steam:hex` do jogador. Caso a `steam:hex` do jogador for diferente da cadastrada no `user_id` que foi feito a tentativa de login, ele faz o banimento automatico daquele jogador.

Dependendo da sua base, talvez seja necessário realizar a troca de algumas funções e até mesmo adaptações no `prepare` da função.

Preview: https://www.youtube.com/watch?v=9jnSpe3O9q4

Créditos:
- Gustavo Pessoa (encontrar onde estava sendo executado o exploit)
- Jhonny Walker (resolver o exploit via server)
