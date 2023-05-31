# Config for Mac M1 and JAVA >= 17
Configuration from scratch. Before start the installation make sure if you're on Hotmart VPN(Forti client) and logged on aws running the following code snippet `hotctl sso login`

## Java version manager
You can you any version manager, but in this doc we're using [sdkMain](https://sdkman.io/install)

Open new terminal and install sdkMain using `curl`

P.S. Installs smoothly on macOS, Linux, WSL, Cygwing, Solaris and FreeBSD. We also support Bash and ZSH shells.

```shell
curl -s "https://get.sdkman.io" | bash
```

Run the follwing code snippet to load sdkmain
```shell
source "$HOME/.sdkman/bin/sdkman-init.sh"
```

Run the follwing code snippet to ensure that installation succeeded
```shell
sdk version
## output should be sdkman >= 5.18.1
```

## SOPS - Secrets OPerationS
If you haven't [sops](https://formulae.brew.sh/formula/sops) installed you can install run the code snippet below.

SOPS is an editor encrypted files that supports YAML, JSON, ENV, INI and BINARY formats and encrypts with AWS KMS, GCP KMS, Azure KEY Vault, age and PGP. See [demo](https://www.youtube.com/watch?v=YTEVyLXFiq0)

```shell
brew install sops
```

