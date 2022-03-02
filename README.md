# lvim-corretor

Vale ressaltar que nada mais do que um dicionario, por padrao vem instalado o corretor para ingles, porem podemos instalar o dicionario em portugues e ter acesso ao corretor, eu uso muito para escrever em markdown.

**Frisando que e um arquivo de dicionario então serve para qualquer editor de texto, ou seja, para o vim básico também**

# Instalação lvim

1. Abra o arquivo config.lua (Dentro do lvim `Space` + `L` + `c` também abre o arquivo)
2. Adicione o caminho do plugin em lvim.plugins
```lua
lvim.plugins = {
     -- Pode ter outros plugins aqui 
     {"gitashay/lvim-corretor"}
}
```
3. lvim automaticamente instala os plugins apos salvar o arquivo config.lua
4. Basta setar o spell com o comando `:set spell spelllang=pt` 

# Comandos

Comandos | Saída
---      | ---
]s       | Move o cursor para a próxima palavra "errada" 
[s       | Move o cursor para a palavra "errada" anterior 
zg       | Adiciona a palavra (no dicionario) em que o cursor está em cima.
zug      | Remove a última palavra adicionada no dicionario
z=       | Vê as sugestões para uma palavra certa, e troca se você escolher alguma delas
