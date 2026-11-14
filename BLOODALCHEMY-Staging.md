# BLOODALCHEMY staging server

Open-directory server that listed the three BLOODALCHEMY loader files CrowdStrike reported as staged during the VAPOR PANDA ARTEX campaign (svchost.exe, graphics-hook-filter64.dll, graphics-hook_config.bin). Shodan recorded the listings on ports 21, 80, 3306 and 8907 between 2026-10-24 and 2026-10-29; the host has not been indexed since 2026-10-31. The match is by file name, not hash, and the attribution is CrowdStrike's.

## Shodan

```
http.html:"graphics-hook_config.bin"
http.html:"graphics-hook-filter64.dll"
```

## IPs

```
118.128.151.28
```
