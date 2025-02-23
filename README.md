# comm-hyprland

**A complete Hyprland setup with custom configurations and keybindings.**  


![image](https://github.com/user-attachments/assets/1200d50e-50de-4c74-88b2-4ae0d3273479)


![image](https://github.com/user-attachments/assets/eea6deb0-9975-4387-9f19-f8b4fb256670)


![image](https://github.com/user-attachments/assets/eb589f2f-259c-4fad-a1ed-99ab5af4f3a4)


## About  

`comm-hyprland` is a package that provides a fully configured **Hyprland** environment, including:  

- A **pre-configured** Hyprland setup  
- Essential **customizations** for an optimal workflow  
- Useful **keybindings** for better window management  

This package is designed for users who want a **ready-to-use Hyprland environment** with a smooth experience.

### Installation via `pacman`  

As the project is still in the testing phase, it will be necessary to use the test repository.

Edit the **`/etc/pacman.conf`** file:
```sh
sudo nano /etc/pacman.conf
```
or 

```sh
sudo vim /etc/pacman.conf
```
Add the line below in the file.

```
[community-testing]
SigLevel = PackageRequired
Server = https://repo.communitybig.org/testing/$arch
```
The file repositories must be in the following order.
```
[community-testing]
SigLevel = PackageRequired
Server = https://repo.communitybig.org/testing/$arch

[community-stable]
SigLevel = PackageRequired
Server = https://repo.communitybig.org/stable/$arch

[community-extra]
SigLevel = PackageRequired
Server = https://repo.communitybig.org/extra/$arch

[biglinux-stable]
SigLevel = PackageRequired
Server = https://repo.biglinux.com.br/stable/$arch

```

Now just run the command below for installation.

```sh
sudo pacman -Sy comm-hyprland
```

## Credits  

This project is inspired by the **[dotfiles](https://github.com/mylinuxforwork/dotfiles)** created by **Stephan Raabe**.  
A big thanks to **Stephan Raabe** for his amazing work and contributions to the Hyprland ecosystem!
