# Heroic Games Launcher

This app is a GUI for the tool [Legendary](https://github.com/derrod/legendary), a native alternative to the Epic Games Launcher for Linux.

![heroic-library](https://user-images.githubusercontent.com/26871415/103456736-384bee00-4cf9-11eb-8674-e6fe3b71be61.png)
![heroic-game](https://user-images.githubusercontent.com/26871415/103456735-37b35780-4cf9-11eb-8f07-667a86b96c6c.png)
![heroic-game-install](https://user-images.githubusercontent.com/26871415/103456734-371ac100-4cf9-11eb-8ab3-584e2b097a72.png)

## Dependencies:
- Xterm (installed in most distros. I'll check the default terminal in the future)
- As of version 0.3.0 is not needed to have Legendary installed.

## How to use it:
- Download and install the binary for your distro or the universal AppImage file on the Releases Page;
- install xterm
- If you used Legendary before, it load your library and installed games. If not, it will ask you for Login First. Just follow the instructions.

## Feature availables right now
- Login with an existing Epic Games account
- Logout
- See the your personal Game library
- Check basic information about your Games
- Install/Uninstall Games
- Play games using the default wine and default prefix
- Sync saves with the cloud (kind of bugged)
- Open game page on Epic Store
- Search for the game on ProtonDB

## Planned features
- Play game with custom wine (Lutris Wine/Proton maybe but can lead to bugs)
- Sync installed games with an existing Epic Games instalation folder
- Import a already installed game
- Get the Free game of the week

## Binaries supported right now
- DEB, RPM, Pacman, AppImage and TAR.XZ (with the heroic binary and all dependecies)
- Might think about Flatpak in the future as well
- There is a AUR version right now: https://aur.archlinux.org/packages/heroic-games-launcher-bin/

## How to build and run locally

This app uses web technologies like Electron, React and Typescript.
To be able to run you will need to have NodeJs installed locally and follow the instructions below:

### Steps:
  - Clone the Repository.
  - Install foreman with `npm i -g foreman`.
  - On the project folder run `npm install`.
  - Run `npm run build` to build the React Assets.
  - Run `npm start`.
  - To build the binaries run `npm run dist`.
