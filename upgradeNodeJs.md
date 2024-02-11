### Mise à jour de Node JS version la dernière version Stable ou Actuel

## assurer vous que NodeJs est déja présent

```bash
node -v
npm -v
```

## MAS 

```bash
sudo npm install -g n
# Pour la version Stable
sudo n stable

#Pour la verison Actuel
sudo n lts

# Vérifie maintenant 
node -v
```

## Si vous avez toujours la même version

Cela est problement lié au chemin de binaire

### Voici la solution

```bash
sudo ln -sf /usr/local/n/versions/node/<Votre_VERSION>/bin/node /usr/bin/nodejs
hash -r

# Vérifions maintenant
node -v
```

#### Si vous avez toujours le même problème modifier ce fichier

```bash
#Ouvrir le fichier avec vim

vim ~/.bashrc
```

#### Rajouter la ligne suivante à la fin de fichier

```bash
export PATH="/usr/local/bin:$PATH"

```

#### Pour que les modifications prennent effet, exécuter la commande suivante:

```bash
source ~/.bashrc
```
