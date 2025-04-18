# rm

> Remove arquivos ou diretórios.
> Veja também: `rmdir`.
> Mais informações: <https://www.gnu.org/software/coreutils/manual/html_node/rm-invocation.html>.

- Remove arquivos específicos:

`rm {{caminho/para/arquivo1 caminho/para/arquivo2 ...}}`

- Remove arquivos específicos ignorando os inexistentes:

`rm {{[-f|--force]}} {{caminho/para/arquivo1 caminho/para/arquivo2 ...}}`

- Remove arquivos específicos interativamente avisando antes de cada remoção:

`rm {{[-i|--interactive]}} {{caminho/para/arquivo1 caminho/para/arquivo2 ...}}`

- Remove arquivos específicos imprimindo informações sobre cada remoção:

`rm {{[-v|--verbose]}} {{caminho/para/arquivo1 caminho/para/arquivo2 ...}}`

- Remove arquivos e diretórios específicos recursivamente:

`rm {{[-r|--recursive]}} {{caminho/para/arquivo_ou_diretório1 caminho/para/arquivo_ou_diretório2 ...}}`

- Remove diretórios vazios (este é considerado o método seguro):

`rm {{[-d|--dir]}} {{caminho/para/diretório}}`
