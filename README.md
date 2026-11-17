# Test

Projet « Hello World » minimal en Rust : le programme affiche simplement `Hello, world!` dans le terminal. Il sert de point de départ pour vérifier l'installation de la chaîne d'outils Rust et la structure de base d'un projet Cargo.

## Prérequis

- [Rust](https://www.rust-lang.org/tools/install), installé via `rustup` (voir ci-dessous)

## Installation de Rust sur Ubuntu

La méthode recommandée est `rustup`, l'installateur officiel, qui fournit la dernière version stable de Rust (le paquet `rustc` d'APT est souvent en retard de plusieurs versions).

1. **Installer les dépendances système** : `curl` pour télécharger l'installateur, et `build-essential` qui fournit l'éditeur de liens (`cc`) nécessaire à la compilation :

   ```sh
   sudo apt update
   sudo apt install -y curl build-essential
   ```

2. **Télécharger et lancer l'installateur `rustup`** :

   ```sh
   curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
   ```

   Quand l'installateur le demande, choisir l'option `1) Proceed with standard installation` (touche Entrée). Rust est installé dans `~/.cargo` et `~/.rustup`, sans droits administrateur.

3. **Charger les variables d'environnement** dans le terminal courant (les nouveaux terminaux le font automatiquement) :

   ```sh
   source "$HOME/.cargo/env"
   ```

4. **Vérifier l'installation** :

   ```sh
   rustc --version
   cargo --version
   ```

   Chaque commande doit afficher un numéro de version.

5. **Mettre à jour Rust** plus tard :

   ```sh
   rustup update
   ```

Pour désinstaller Rust : `rustup self uninstall`.

## Utilisation

```sh
cargo run
```

## Structure

- `Cargo.toml` : configuration du projet (nom, version, dépendances)
- `src/main.rs` : point d'entrée du programme
