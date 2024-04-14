# change config permission
mkdir -p ~/nixos-config
sudo mv /etc/nixos/configuration.nix ~/nixos-config/
sudo ln -s /home/sourav/nixos-config/configuration.nix /etc/nixos/configuration.nix
ls -l /etc/nixos/configuration.nix
chmod 600 ~/nixos-config/configuration.nix
id -gn sourav -> check group
sudo chown sourav:users ~/nixos-config/configuration.nix
sudo nixos-rebuild switch


# add python path to pycharm
which python3 -> use this path to provide to pycharm

