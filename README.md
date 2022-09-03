# docker-container-cpu-memory-usage

## 📖 Descrição do Projeto ##
> **Verifica a utilização de CPU e memória RAM de um ou mais containers *Docker* a partir de uma(s) imagem/imagens especificada(s) e escreve em um arquivo `.csv`.**
> <br />
> **Você pode mesclar os arquivos `.csv` utilizando o [csv-merge](https://github.com/AllanCapistrano/csv-merge).**

### 📦 Dependências: ###
- [Command](https://pypi.org/project/Command/)
- [psutil](https://pypi.org/project/psutil/)
- [python-dotenv](https://pypi.org/project/python-dotenv/)

------------

## 💻 Como utilizar o projeto e/ou modificá-lo ##

1. Faça um Fork deste repositório (caso queira modificá-lo) ou somente clone-o.
2. Acesse o diretório do projeto;
3. Instale as dependências do projeto:
   ```powershell
   pip install -r requirements.txt
   ```
   Ou
   ```
   # Linux/macOS
   python3 -m pip install -r requirements.txt
   ```
4. Defina as variáveis de ambiente:
   ```powershell
   cp .env.example .env
   ```
5. Execute o projeto:
   ```powershell
   python3 src/main.py
   ```

### Variáveis de amviente
- `HEADER`: Lista contendo o cabeçalho da tabela. 
   - Obs: é necessário seguir o padrão definido no arquivo `.env.example`;
- `IMAGE_NAMES`: Lista contendo o nome da(s) imagem/imagens *Docker* que se deseja monitorar;
- `SLEEP_CSV_WRITER_THREAD`: Intervalo de tempo em **segundos** que a *thread* irá escrever os dados no arquivo `.csv`;
- `SLEEP_STATS_THREAD`: Intervalo de tempo em **segundos** que a *thread* irá monitorar o *gateway*;
  - Obs: Esse valor deverá ser menor que o definido em `SLEEP_CSV_WRITER_THREAD`;
------------

## 🤝 Contribuições ##

### Sinta-se a vontade para contribuir com este projeto. ###

1. Faça um *Fork* deste repositório;
2. Cria sua *branch*:
   ```powershell
   git checkout -b my-new-feature
   ```
3. *Commit* suas modificações:
   ```powershell
   git commit -m "Add some feature"
   ```
4. Faça o *push* na sua *branch*:
   ```powershell
   git push
   ```
   Ou
   ```powershell
   git push origin my-new-feature
   ```

------------

## 👨‍💻 Autor ##

| [![Allan Capistrano](https://github.com/AllanCapistrano.png?size=100)](https://github.com/AllanCapistrano) |
| -----------------------------------------------------------------------------------------------------------|
| [Allan Capistrano](https://github.com/AllanCapistrano)                                                     |

<p>
    <h3>Onde me encontrar:</h3>
    <a href="https://github.com/AllanCapistrano">
        <img src="https://github.com/AllanCapistrano/AllanCapistrano/blob/master/assets/github-square-brands.png" alt="Github icon" width="5%">
    </a>
    &nbsp
    <a href="https://www.linkedin.com/in/allancapistrano/">
        <img src="https://github.com/AllanCapistrano/AllanCapistrano/blob/master/assets/linkedin-brands.png" alt="Linkedin icon" width="5%">
    </a> 
    &nbsp
    <a href="https://mail.google.com/mail/u/0/?view=cm&fs=1&tf=1&source=mailto&to=asantos@ecomp.uefs.br">
        <img src="https://github.com/AllanCapistrano/AllanCapistrano/blob/master/assets/envelope-square-solid.png" alt="Email icon" width="5%">
    </a>
</p>

------------

## 🙏 Apoie ##

**Por favor ⭐️ este repositório caso este projeto seja útil e/ou tenha lhe ajudado.**

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/allancapistrano)

------------

## ⚖️ Licença ##
[GNU General Public License v3.0](./LICENSE)
