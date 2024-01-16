setup nix for WSL2 Ubuntu

zero-to-nix
```url
https://zero-to-nix.com/start/install
```

home-manager
```url
https://nix-community.github.io/home-manager/index.xhtml#sec-install-standalone
```

if home-manager failed to complete installation, please follow this thread
```url
https://github.com/nix-community/home-manager/issues/4879
```

Adding package to home.nix
go to ~/.config/home-manager/home.nix

update this following line
```nix
home.packages = [
    pkgs.nodejs_21
]
``` 

for pkgs you can find it here
```url
https://search.nixos.org/packages
```

Adding program to home.nix
```nix
programs.fish = {
    enable = true;
    plugin = [
        # your plugin object
        
    ]
}
```

for programs, you can find it here
```url
https://mipmip.github.io/home-manager-option-search/
```