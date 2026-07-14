# Desafio-Phishing-Dio
Repositório de armazenamento do passo a passo da criação do pishing usando clone de página por meio do setoolkit
## Ferramentas
*  Kali Linux
*  setoolkit

## Como configurar o phishing no Kali Linux
* Acesso root: ```sudo su```
* Iniciar o setoolkit: ```setoolkit```
* Selecionar o tipo de ataque: ```Social-Engineering Attacks```
* Selecione o tipo de ataque de engenharia social por website: ```Website Attack Vectors```
* Selecione o tipo de web ataque: ```Credential Harvester Attack Method```
* Selecione o tipo de método clonador de site: ```site cloner```
* Informe o endereço do servidor que ficará a página clonada: ```ex.: 10.0.1.10```
* Página website clonada: http://www.facebook.com/
<img width="1918" height="908" alt="image" src="https://github.com/user-attachments/assets/dedf0f1a-f626-4e4b-8147-67f268cb8fbc" />
Foi seguido todo o passo a passo da resolução porém a página apresentou proteção contra a ferramenta setoolkit

## Solução
Criei uma página login em html e subi ela para a rede local usando um servidor http python com ip, porta e pasta da página eu informei no setoolkit e então consegui realizar o clone da página
<img width="720" height="151" alt="image" src="https://github.com/user-attachments/assets/837f4a71-c9ec-4a0a-ad09-0433e2d2ebc0" />
<img width="1903" height="953" alt="image" src="https://github.com/user-attachments/assets/176ff32c-cdec-4e85-9ed7-c0ae0437b4cf" />

* Criar página login
* Dentro do terminal, estando na pasta do arquivo, executar o comando ```python -m http.server 8000```
* O arquivo deve estar nomeado como **index.html**
* Após confirmar que a página está acessível na rede local, pegue as informações do link dela como ip, porta e pasta e coloque no setoolkit e execute o clone

Página com o link original gerado pelo servidor http python
<img width="1903" height="953" alt="image" src="https://github.com/user-attachments/assets/1fbc6aa8-e0b2-4370-8bd3-f11d84bc3369" />

Página **phishing** usando o setoolkit
<img width="1907" height="958" alt="image" src="https://github.com/user-attachments/assets/231b8c32-8956-4361-bfc2-c8c344c0bb56" />

Terminal do Kali Linux:
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/6de694a1-c59e-4a49-93e2-e9568fa9fe2e" />


