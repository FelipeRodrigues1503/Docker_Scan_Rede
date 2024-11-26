 # Scan de rede utilizando imagem Docker

Este projeto implementa um script shell para realizar varreduras de rede utilizando o `nmap`. 
Contendo também um arquivo Dockerfile configurado para executar o script em um ambiente baseado no Alpine Linux instalando automaticamente todas as dependências necessárias.

*scan_rede.sh*:
  1. Solicita ao usuário o intervalo de rede a ser escaneado.
  2. Realiza a varredura de portas usando o `nmap`.
  3. Salva os resultados da varredura em um arquivo de texto.
  4. Permite o enviar o arquivo.txt dos resultados por e-mail via SMTP.
  
- **Dockerfile**: Configura um contêiner baseado no Alpine Linux:
  1. Instala todas as dependências
  2. Executa automaticamente o script

Após clonar o repositorio, crie uma imagem no repositorio clonado:
  docker build -t (nome_imagem) .
  
  Executando a imagem criada:
  docker run -it (nome_imagem)
