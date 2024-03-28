# Workshop : Intéragir avec la blockchain en Go
Dans ce workshop, vous apprendrez comment interagir simplement avec la blockchain en utilisant "Go Ethereum", l'implémentation officielle d'Ethereum en Go.
> ▶️ Repo officiel [ici](https://github.com/ethereum/go-ethereum/)  
> ❗ Documentation [go-ethereum](https://goethereumbook.org)

## Partie 0 : Setup
Installe Go en suivant la [documentation officielle](https://go.dev/doc/install)    

## Partie 1 : Récupérer des informations

### Etape 1 : Numéro d'un Block
Maintenant que tout est installé. Essayez de lancer le code déjà présent dans votre repo pour la première fois :
```shell
go run ./part1
```
Pour l'instant, il ne se passe rien.  

__Votre but est ici est de `print` le numéro du dernier `block` miné de la chaine.__
  
> Essayez de comprendre, dans un premier temps, ce que fait le code que vous venez d'éxecuter. 😉
  
> La [documentation](https://pkg.go.dev/github.com/ethereum/go-ethereum/ethclient) d'un `client` en go-ethereum

> [Print en Go](https://pkg.go.dev/fmt#example-Println) 

> Vous pouvez vérifier le numéro du dernier block [ici](https://etherscan.io/) dans la catégorie "Latest blocks"

### Etape 2 : Solde d'un wallet
Toujours dans le même style, __vous devez cette fois-ci récupérer le solde (en Ether) d'un wallet__ (à choisir [ici](https://etherscan.io/)).  
(Attention, la valeur devra être convertie 😉)

> Une address ne peut pas être utiliser directement depuis sa string => ⚠️ [Doc](https://pkg.go.dev/github.com/ethereum/go-ethereum/common#HexToAddress)
  
> [Convertisseur](https://www.alchemy.com/gwei-calculator) 

## Partie 2 : Créer un wallet sécurisé

### Etape 1 : Générer un wallet simple
__Générez et print une `private key` ainsi que sa `public key` et sa `public address`.__

Vous aurez ainsi les trois informations principales constituant votre premier wallet.

> [Comment sont générées les clés d'un wallet](https://www.dynamic.xyz/blog/everything-you-wanted-to-know-about-wallet-keys#generating-the-keys)

### Etape 2 : Générer un keystore (Encrypted Wallet)
Bravo, vous venez de créer votre wallet...mais il n'est pas sécurisé du tout. En effet, la clé privée n'est pas cryptée.  
__Utilisez le système de `keystore` (ou `Encrypted Wallet`) pour générer un wallet.__   
Il sera sous forme d'un fichier contenant toutes les informations cette fois-ci cryptée

> Qu'est-ce qu'un [keystore](https://support.token.im/hc/en-us/articles/360002074313-What-is-a-keystore) ?
  
> Générez votre keystore dans le dossier `wallet`

### Etape 3 : Décrypter un keystore
Affichez la `private key`, la `public key` et la `public address` du keystore que vous venez de créer.

## Partie 3 : Faire des transactions
A partir d'ici, nous allons intéragir avec le testnet `Sepolia` afin de faire des transactions de `Sepolia Eth`
> Qu'est-ce qu'un [testnet](https://cryptoast.fr/qu-est-ce-qu-un-testnet-blockchain/)
  
### Etape 1 : Nouveaux wallets
__Générez deux nouveaux `wallets` et récupérez leur `public address`__

### Etape 2 : Récupérer leur solde
A l'image de la Partie 1, __récupérez le solde de vos deux wallets__

> Vous pouvez trouver les informations de vos wallets sur le testnet [ici](https://sepolia.etherscan.io/)
  
### Etape 3 : Effectuer une transaction
__Créez, signez et envoyez votre première transaction de `Sepolia Eth` d'un wallet à un autre.__

> Récupérez des `Sepolia Eth` en les [minant](https://sepolia-faucet.pk910.de/) (Copiez/collez l'addresse public précédé de '0x') ou appellez moi, je pourrais surement en envoyer pour allez plus vite.
  
> Affichez le hash de votre transaction afin de la retrouver facilement [ici](https://sepolia.etherscan.io/)

## Pour aller plus loin
- Apprendre à écrire des smart contracts en Solidity (s/o Geoffrey, un workshop devrait arriver pour ça)
- Utiliser le Go afin de déployer ces smart contracts sur un Testnet Ethereum
- Intéragir avec ses smart contracts en utilisant le Go
