# Estudo-de-Git-

Manipulação de histórico git



| Comando                       | Definição                                                                                                                                                     |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `git commit --amend`          | Altera o último commit, permitindo corrigir sua mensagem ou incluir alterações esquecidas.                                                                    |
| `git rebase -i`               | Permite reorganizar, editar, juntar, renomear ou remover commits existentes no histórico.                                                                     |
| `git reset --soft`            | Remove o commit do histórico, mas mantém as alterações preparadas (*staged*).                                                                                 |
| `git reset --mixed`           | Remove o commit e mantém as alterações no diretório de trabalho, mas fora do *staging*.                                                                       |
| `git reset --hard`            | Remove o commit e descarta as alterações associadas. Deve ser usado com muito cuidado.                                                                        |
| `git revert`                  | Cria um novo commit que desfaz as alterações de um commit anterior, preservando o histórico.                                                                  |
| `git reflog`                  | Mostra referências anteriores do `HEAD`, sendo muito útil para recuperar commits ou estados aparentemente perdidos.                                           |
| `git push --force-with-lease` | Atualiza uma branch remota sobrescrevendo o histórico remoto, mas com uma verificação de segurança para evitar sobrescrever alterações novas de outra pessoa. |

### Para memorizar

| Comando            | Pense em...                                  |
| ------------------ | -------------------------------------------- |
| `amend`            | **Corrigir o último**                        |
| `rebase`           | **Reorganizar o histórico**                  |
| `reset`            | **Voltar a branch**                          |
| `revert`           | **Desfazer criando outro commit**            |
| `reflog`           | **Encontrar estados anteriores**             |
| `force-with-lease` | **Atualizar histórico remoto com segurança** |


Situação	Comando	Palavra para memorizar
Corrigir o último commit	git commit --amend	✏️ ARRUMAR
Organizar commits	git rebase -i	🧹 ORGANIZAR
Voltar a branch	git reset	🔙 VOLTAR
Desfazer mantendo histórico	git revert	🔄 DESFAZER
Procurar estados anteriores	git reflog	🧠 LEMBRAR

🧠 Frase mágica

AMEND arruma. REVERT desfaz.

Comando	O que acontece	🧠 Palavra
git reset --soft	Volta e mantém as alterações em staged	🟢 Segura
git reset --mixed	Volta e mantém as alterações, mas fora do staging	🟡 Solta
git reset --hard	Volta e descarta as alterações	🔴 Joga fora

✏️ amend → corrigir o último commit
🧹 rebase -i → organizar o histórico
🔙 reset → voltar a branch
🔄 revert → desfazer mantendo o histórico
🧠 reflog → consultar a memória do Git
🟢 reset --soft → voltar mantendo staged
🟡 reset --mixed → voltar mantendo as alterações fora do staging
🔴 reset --hard → voltar descartando alterações

