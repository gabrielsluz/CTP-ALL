# CTP-All

Neste repositório estão as implementações dos protocolos de coleta de dados para plataformas de dois rádios PAC-A, PAC-I e CTP-Multi. Os protocolos foram apresentados no artigo " PAC-A e PAC-I : Protocolos de Árvore de Coleta para Plataformas com Dois Rádios". Também estão aqui o código fonte da aplicação usada para fazer os experimentos, os programas usados para agregar os resultados e o script em python para automatizar o envio de testes para o testbed.

# Código fonte

Dentro das pastas com os nomes dos protocolos está o código fonte para o TinyOS na plataforma Opal. A pasta "ctp" contém a principal parte de cada protocolo. Já a pasta "TestCtp" contém a aplicação usada para fazer os experimentos.

# Reprodução dos experimentos

Para reproduzir os experimentos entre na pasta "TestCtp". Para alterar os parâmetros usados (período de geração de pacotes e duração do experimento) altere as constantes definidas no início do arquivo "TestCtpC.nc". Para criar a imagem executável digite o comando no terminal: "make opal", e será criada uma imagem no diretório "build/opal". Os dados coletados no experimento são coletados pelo "SerialLogger" e as constantes que indexam essa coleta estão no arquivo "TestCtp.h".
