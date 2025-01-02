## Enviroment
```
bash <(curl -s https://octra.j-node.net/octra_enviroment.sh)
```

```
eval $(opam env)
```
```
wget https://octra.j-node.net/config.ml
```
```
ocamlfind ocamlopt -o config -thread -linkpkg -package yojson,cohttp-lwt-unix,unix,str,lwt_ppx config.ml
```
## Config Validator info to get hash for launch validator node:
```
./config
```
## Validator map:
http://161.35.168.80:9001/

## Output sample:
```
⚡ root@josephtran  ~  ocamlfind ocamlopt -o config -thread -linkpkg -package yojson,cohttp-lwt-unix,unix,str,lwt_ppx config.ml
 ⚡ root@josephtran  ~  ./config
ℹ Detecting operating system...
✓ Detected OS: Linux.

╺━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╸
              Octra node configurator              
╺━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╸

Upon successful configuration, you will receive a configuration file
containing your unique validator hash. This file will be required
when launching your validator node.


→ Personal information

→ Validator name (nickname or organization): J-Node
✓ Input successfully validated.


→ Validator website (optional): www.j-node.net
✓ Input successfully validated.


→ Contact email: josephtran0505@gmail.com
✓ Input successfully validated.



→ Contacts

→ Telegram account: josephtran
✓ Input successfully validated.


→ Discord nickname: josephtran
✓ Input successfully validated.



→ Server configuration

→ Server location (City, Country): Vienna, Austria
✓ Input successfully validated.


→ Cluster (will there be multiple servers? y/n): n
✓ Input successfully validated.


→ Planned uptime (hours per day): 24
✓ Input successfully validated.


→ IP address type (static/non-static): static
✓ Input successfully validated.


→ Available disk space (MB): 3000000   
✓ Input successfully validated.



→ System information collection
ℹ Getting OS information...
✓ OS information collected successfully..
ℹ Extracting CPU features and capabilities...
✓ CPU information and capabilities collected successfully..
ℹ Collecting memory information...
✓ Memory information collected successfully..
ℹ Getting local IP address...
✓ Local IP collected successfully..
ℹ Getting external IP address...
✓ External IP collected successfully..

→ Creating configuration
ℹ Preparing configuration data...
ℹ Registering server in the Octra Network...


*****************************************
| Configuration successfully completed. |
*****************************************

Configuration details:
• Hash ID: 2dc6e74298bfd21fa9f6f080d44215be
• File: 2dc6e74298bfd21fa9f6f080d44215be_config.json
Your configuration has been saved locally and the authorization actor has registered this account in the network

╺━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╸
              Setup Complete              
╺━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━╸
```
