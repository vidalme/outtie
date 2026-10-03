# Outtie — espaço individual

Este modelo não contém dados pessoais nem um ciclo ativo. O setup do `innie` inicializa ou valida os metadados e cria o link de acesso. Fontes, evidências, planos, versões e archives pertencem a este espaço.

## Uso

Dentro do `innie`, executar `python3 scripts/pdi.py setup`. Para conectar esta pasta em outra localização, usar `python3 scripts/pdi.py --outtie CAMINHO connect`.

Não editar metadata.json ou revisions manualmente. Usar propostas e scripts. O schema é 1; formatos antigos desconhecidos não são sobrescritos. A documentação completa está no repositório `innie`.

## Git opcional

`python3 scripts/pdi.py init-git` inicializa Git neste espaço. Não faz commit, configura remote ou envia conteúdo. Se for publicar, selecionar um repositório privado autorizado e conferir tudo o que será enviado. `.runtime` e backups locais são ignorados; os demais documentos individuais podem ser rastreados deliberadamente.

## Recuperação

Manter backup verificado fora desta pasta/disco quando possível. Restaurar em destino novo e reconectar. As revisões ajudam a recuperar mudanças, mas não substituem backup do ambiente WSL.

Dados locais usados pelo Copilot podem ser enviados ao serviço de IA. Este espaço não garante isolamento de rede ou controle de acesso apenas por estar separado do innie.
