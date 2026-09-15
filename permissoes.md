# Permissões Linux e princípio do menor privilégio

Esta atividade teve como objetivo praticar permissões de ficheiros em Linux e compreender a sua relação com segurança e controlo de acessos.

## Ficheiros utilizados

- **publico.txt** — ficheiro destinado a leitura pública.
- **restrito.txt** — ficheiro com acesso limitado ao proprietário e ao grupo.
- **script.sh** — script com permissão de execução atribuída de forma controlada.

## Permissões aplicadas

| Ficheiro | Permissão | Justificação |
|---|---:|---|
| `publico.txt` | `644` | Todos podem ler, mas apenas o proprietário pode escrever. |
| `restrito.txt` | `640` | Proprietário pode ler/escrever, grupo pode ler e outros não têm acesso. |
| `script.sh` | `u+x` | A execução é concedida ao proprietário sem abrir a permissão a todos os utilizadores. |

## Interpretação

### `644`

- Proprietário: leitura e escrita.
- Grupo: leitura.
- Outros: leitura.

É adequado para conteúdo que pode ser consultado por vários utilizadores, mas cuja alteração deve permanecer controlada.

### `640`

- Proprietário: leitura e escrita.
- Grupo: leitura.
- Outros: sem acesso.

É mais apropriado para informação que não deve ficar disponível a qualquer utilizador do sistema.

### `u+x`

Adiciona permissão de execução apenas ao proprietário do ficheiro. Em vez de conceder execução globalmente, limita-se o privilégio ao utilizador que realmente necessita dele.

## Relação com o princípio do menor privilégio

O **princípio do menor privilégio** estabelece que cada utilizador ou processo deve receber apenas as permissões necessárias para executar a sua função.

Neste laboratório, evitar permissões excessivas como `777` reduz o risco de:

- alterações não autorizadas;
- execução indevida de ficheiros;
- exposição desnecessária de informação;
- utilização abusiva de recursos do sistema.

## Conclusão

A configuração correta de permissões é uma medida básica, mas essencial, de segurança em Linux. O objetivo não é dar o máximo de acesso possível, mas sim conceder **apenas o acesso necessário** para cada situação.
