Missão Aquário Digital
Protocolo de Versionamento e Gestão de Ecossistema

Este projeto faz parte da atividade de Garantia da Qualidade de Software e tem como objetivo simular um fluxo profissional de desenvolvimento utilizando Git e GitHub.

O sistema possui um módulo responsável pelo monitoramento da qualidade da água de um aquário, verificando os níveis de pH e temperatura.

Camadas do Ambiente
Develop

A branch develop é utilizada para o desenvolvimento e integração das novas funcionalidades do sistema.

Stage

A branch stage representa o ambiente de testes e homologação. As funcionalidades desenvolvidas são validadas nessa etapa antes de serem disponibilizadas em produção.

Main

A branch main representa o ambiente de produção. Somente funcionalidades aprovadas e validadas na stage devem ser promovidas para essa branch.

Módulo de Controle da Qualidade da Água

O módulo ControleQualidadeAgua.java realiza o monitoramento de dois parâmetros da água:

pH: considerado ideal entre 6.8 e 7.6.
Temperatura: considerada segura entre 22°C e 28°C.

Quando algum parâmetro está fora dos limites definidos, o sistema apresenta uma mensagem de alerta. Quando os parâmetros estão dentro dos limites, o sistema informa que a água está em níveis ideais.

Responsáveis
Biólogo/Desenvolvedor: Caio Duraes Vasconcelos
Fluxo de Desenvolvimento
feature/controle-qualidade
            ↓
         develop
            ↓
          stage
            ↓
          main