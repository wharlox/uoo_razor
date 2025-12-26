# uoo_razor

a backup of some of my stuff


git add active chain-scripts:
```
awk -F'[\\\\ ]'  '!/#/ && /functions/  {gsub(/"|\r/,""); print $NF}'  deposit-mine-test-chain.razor | xargs -I{} git add functions/{}.razor
```
