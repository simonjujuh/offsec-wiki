# RDP 

Port: 3389

## Clients

```bash
# XfreeRDP
xfreerdp /v:"$TARGET" /d:"$DOMAIN" /u:"$USER" /p:"$PASSWORD" /cert-ignore /dynamic-resolution
xfreerdp /v:"$TARGET" /d:"$DOMAIN" /u:"$USER" /p:"$PASSWORD" /cert-ignore /drive:"${SHARENAME},${LOCALPATH}"
xfreerdp /v:"$TARGET" /d:"$DOMAIN" /u:"$USER" /pth:"$NT_HASH" /cert-ignore # PTH

# L'accès au share se fait avec le chemin UNC suivant
\\tsclient\SHARE\file.txt
```
