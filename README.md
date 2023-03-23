# Update Warning

> Caso tenha updates em seu script avisar o seu cliente.

> Developed by: Vieira's Store

> Framework: Standalone

# Como usar?

**Crie dois pastbins utlizando o site: https://pastebin.com (Recomendado), Um voce irá colocar a versão do script sendo executada, Ja no outro será a mesma versão porem vai ser nesse pastbin que voce ira atualizar quando tiver algum update no codigo. Lembrando que o que esses pastbins devem conter serão numeros especificando as versões EX: 1^ 123032023 no outro, Que seria o de atualização 223032023 que seria uma versão diferente. O Script irá verificar se a versão do script é igual a versão atualizada, Se for ele não printa nada, Agora, Se for diferente ele irá printar que tem uma nova versão do codigo.**

# Codigo

> 🟢Versão estavel

```lua
PerformHttpRequest("PASTEBIN COM A VERSÃO DO SCRIPT",function(err, data)
    local resName = GetCurrentResourceName()
    if err >= 200 and err <= 299 then
        local script_version = data
        PerformHttpRequest("PASTEBIN QUE VOCE IRA ATUALIZAR A VERSÃO DO SCRIPT",function(err2, data2)
            if err2 >= 200 and err2 <= 299 then
                local script_version_updated = data2
                if script_version == script_version_updated then
                else
                    print("^3["..resName.."] Para novas features e correcoes de bugs, Reinstale o script.^0")
                end
            end
        end)
    end
end)
```

# Contato
- Comercial: contato.vsdev@gmail.com 🧾
- Discord: https://discord.gg/C5tXDsZhVJ 🧾
- Website: https://sites.google.com/view/vieiras-store/home 🧾
