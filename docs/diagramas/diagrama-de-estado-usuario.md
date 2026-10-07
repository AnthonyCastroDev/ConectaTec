# Diagrama de Estado - Usuário

```mermaid
stateDiagram-v2
    [*] --> Cadastrado : Realiza cadastro
    Cadastrado --> Autenticado : Login válido
    Autenticado --> Cadastrado : Logout
    Autenticado --> PerfilCompleto : Preenche o perfil
    PerfilCompleto --> Autenticado : Edita o perfil
    PerfilCompleto --> Cadastrado : Logout
    Cadastrado --> Inativo : Desativa a conta
    Autenticado --> Inativo : Desativa a conta
    Inativo --> [*]
```
