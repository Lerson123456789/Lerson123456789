graph TD
    A(Início) -->|Carregar Estudantes e Docentes| B(Menu Principal)
    B -->|tipo_usuario = 1| C(Subfluxo Estudante)
    B -->|tipo_usuario = 2| D(Subfluxo Docente)
    B -->|tipo_usuario = 3| E(Fim)

    C -->|opcao = 1| F(Cadastrar Estudante)
    C -->|opcao = 2| G(Autenticar Estudante)
    C -->|opcao = 3| E

    D -->|opcao = 1| H(Cadastrar Docente)
    D -->|opcao = 2| I(Autenticar Docente)
    D -->|opcao = 3| E

    F --> C
    G --> C
    H --> D
    I --> D

