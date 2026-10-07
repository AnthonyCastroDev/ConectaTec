# Diagrama de Casos de Uso

```mermaid
flowchart LR
    aluno([Aluno])
    empresa([Empresa])

    subgraph Sistema[ConectaTec]
        uc1([Cadastrar-se])
        uc2([Fazer login])
        uc3([Editar perfil])
        uc4([Cadastrar habilidades])
        uc5([Gerenciar projetos])
        uc6([Buscar alunos e empresas])
        uc7([Visualizar perfil])
        uc8([Conectar-se])
    end

    aluno --- uc1
    aluno --- uc2
    aluno --- uc3
    aluno --- uc4
    aluno --- uc5
    aluno --- uc6
    aluno --- uc7
    aluno --- uc8

    empresa --- uc1
    empresa --- uc2
    empresa --- uc3
    empresa --- uc6
    empresa --- uc7
    empresa --- uc8
```
