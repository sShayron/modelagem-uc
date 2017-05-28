# Modelagem/Diagrama de Casos de Uso

## Em que fase do processo de desenvolvimento de um software é utilizado a modelagem de u.c ?
Após a elicitação, analise e especificação, e validação dos requisitos, é feito os casos de uso na documentação dos requisitos.


## O que é o caso de uso?
Esse diagrama descreve uma sequencia de ações, das funcionalidades prinicipais, no sistema no ponto de vista do usuário. Aqui não é abordado detalhes técnicos de como o sistema funcionará.


## Qual objetivo da modelagem de caso de uso?
Visa simplificar o entendimento por parte do usuário de como o sistema funcionará.


## Quais são os elementos de um diagrama de caso de uso?
- **Cenário**: Sequência de eventos que acontecem quando um usuário interage com o sistema.
- **Ator**: Usuário do sistema, ou melhor, um tipo de usuário.
- **Use Case**: É uma tarefa ou uma funcionalidade realizada pelo ator (usuário).
- **Relacionamentos**: É o que liga um ator com um caso de uso.


## Possiveis _atores_ de um diagrama de caso de uso
Considerando um sistema de consultório médico, podemos considerar atores:
* Secretária
* Médico
* Paciente


## Tipos de relacionamentos existentes em um diagrama de caso de uso e possiveis agentes
* **Include**: seria a relação de um caso de uso que para ter sua funcionalidade executada precisa chamar outro caso de uso.
* **Extend**: Esta relação significa que o caso de uso extendido vai funcionar exatamente como o caso de uso base só que alguns passos novos inseridos no caso de uso extendido.
Por exemplo 'visualizar consultas' seria um include para o ator secretária e alterar consulta um extend, pois o alterar seria executado após visualizar.


## Exemplos de caso de uso
Exemplo de caso de uso de uma secretária num sistema de representantes

![UC](/uc1.png)


## Diferença entre relacionamento de _include_ e _extend_
O extend é uma ação executada só após um include, o include está relacionado diretamente com o ator, já o extend não.


## Possiveis relacionamentos de herança entre _atores_
Em um sistema bancário por exemplo, o caixa, cliente e gerente podem ter o mesmo caso de uso de um usuário comum (ator genérico). 

![Herança ator](/heranca_usuario.png)


## Possiveis relacionamentos de herança entre _casos de uso_
"Exibir saldo impresso" ou na tela, herda de "exibir saldo".

![Herança UC](/heranca_uc.png)
