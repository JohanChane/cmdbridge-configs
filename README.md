# CmdBridge Configs

## Usage

```sh
git clone https://github.com/JohanChane/cmdbridge-configs.git --depth 1
cd cmdbridge-configs
./install
cmdbridge cache refresh
```

## Use Scripts

Add to `zshrc`:

```sh
export PATH="${XDG_CONFIG_HOME:-$HOME/.config}/cmdbridge/scripts":PATH
```

## list all

```sh
cmdbridge list all
```

Output:

```
## firewall
                       iptables    mufw   
------------------------------------------
allow_ip                  ✓         ✓     
allow_port                ✓         ✓     
allow_service             ✓         ✓     
delete_allow_ip           ✓         ✓     
delete_allow_port         ✓         ✓     
delete_allow_service      ✓         ✓     
delete_deny_ip            ✓         ✓     
delete_deny_port          ✓         ✓     
delete_deny_service       ✓         ✓     
deny_ip                   ✓         ✓     
deny_port                 ✓         ✓     
deny_service              ✓         ✓     
disable_firewall          ✓         ✓     
enable_firewall           ✓         ✓     
reset                     ✓         ✓     
status                    ✓         ✓     

## package
                                           apt       brew     cargo      dnf       npm      pacman     pip      zypper  
------------------------------------------------------------------------------------------------------------------------
download_source                             ✓         ✓         ✗         ✓         ✓         ✓         ✓         ✓     
find_file_owner_with_regexp                 ✓         ✓         ✗         ✓         ✗         ✓         ✗         ✓     
info                                        ✓         ✓         ✓         ✓         ✓         ✓         ✓         ✓     
install                                     ✓         ✓         ✓         ✓         ✓         ✓         ✓         ✓     
list_files                                  ✓         ✓         ✗         ✓         ✓         ✓         ✓         ✓     
list_installed                              ✓         ✓         ✓         ✓         ✓         ✓         ✓         ✓     
list_installed_manually_with_my_format      ✓         ✗         ✗         ✗         ✗         ✓         ✗         ✗     
remove                                      ✓         ✓         ✓         ✓         ✓         ✓         ✓         ✓     
search_local                                ✓         ✓         ✗         ✓         ✗         ✓         ✗         ✓     
search_remote                               ✓         ✓         ✓         ✓         ✓         ✓         ✓         ✓     
update_pkg_db                               ✓         ✓         ✗         ✓         ✗         ✓         ✗         ✓     
upgrade_sys                                 ✓         ✓         ✗         ✓         ✗         ✓         ✗         ✓     
```