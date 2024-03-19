## Workshop : Intéragir avec la blockchain en Go
Dans ce workshop, vous apprendrez comment interagir simplement avec la blockchain en utilisant "Go Ethereum", l'implémentation officielle d'Ethereum en Go.
> ▶️ Repo officiel [ici](https://github.com/ethereum/go-ethereum/)

# Etape 0 : Setup
Installe Go en suivant la [documentation officielle](https://go.dev/doc/install)  
Rejoins la [Github Classroom](https://classroom.github.com/a/0C5KsjlB) et suis les indications. Cela te dirigera vers un nouveau repo dans lequel tu vas travailler.  

# Etape 1 : Block number
Maintenant que tout est installé. Essayez de lancer votre code pour la première fois :
```shell
go run ./src
```
Pour l'instant, il ne se passe rien.  
  
__Votre but est ici est de `print` le numéro du dernier `block` miné de la chaine.__
  
> Essayez de comprendre, dans un premier temps, ce que fait le code que vous venez d'éxecuter. 😉
  
> La [documentation](https://pkg.go.dev/github.com/ethereum/go-ethereum/ethclient) d'un `client` en go-ethereum

> [Print en Go](https://pkg.go.dev/fmt#example-Println) 

> Vous pouvez vérifier le numéro du dernier block [ici](https://etherscan.io/) dans la catégorie "Latest blocks"
