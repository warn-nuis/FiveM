---
order: 2
---

# ⚙ Configurações

Aqui você pode aprender como configurar os nossos scripts para não ter problemas técnicos e poder aprender um pouco de programação

# Instalação

!!!Warning Instalação 
Caso nao tenha o script **Painel Staff** instalado na sua base siga o tutorial.
!!!

- No arquivo `config/config.lua` va ate e procure a configuracao na imagem e altere para a sua `Framework` caso a sua base nao correponder com `vrpex / creative / creative_v5 / creative_network` vode pode abrir um ticket no [discord](https://discord.gg/warn-nuis).

![](/images/i1.png)

- Apos fazer a alteraçao da `Framework` voce deve colocar a licença no arquivo `license.json` a licença e enviada pelo `gamboz` na hora da compra do produto.

!!!info  Permissoes 
Ajuste as permissoes para conseguir acessar o **Painel Staff** para que todas as funcoes funcionem !
!!!

- No arquivp `config/config.lua` voce vai reparar que existe varias permissoes para serem colocadas para voce achar isso na sua base voce deve procurar a pasta `vrp` 

```lua
Config.Permissoes = {
    ['Abrir-painel'] = "Admin",
}
```

==- vRPex (groups.lua)
Para voce achar a permissao de `staff` no sua base voce deve ir no arquivo `vrp/cfg/groups.lua`
![](/images/i2.png)
- Exemplo o meu seria o `admin.perm`
```lua
cfg.groups = {
	["Dono"] = {
		_config = {
			title = "Dono",
			gtype = "staff"
		},
		"dono.perm",
		"admin.perm",
		"mod.perm",
	},
}```
===

==- Creative (groups.lua)
Para voce achar a permissao de `staff` no sua base voce deve ir no arquivo `vrp/modules/group.lua`
![](/images/i4.png)
- Exemplo o meu seria o `Admin`
```lua
local permissions = {
	["Admin"] = {
		["Admin"] = true,
	},
}```
===



