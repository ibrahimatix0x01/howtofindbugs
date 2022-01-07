# howtofindbugs
[![](https://img.shields.io/twitter/follow/ibrahimatix_?color=blue&label=Twitter&logo=twitter&style=plastic)](https://twitter.com/ibrahimatix_)&nbsp;&nbsp;
[![](https://img.shields.io/github/followers/ibrahimatix?color=gray&label=GitHub&logo=github&style=plastic)](https://github.com/ibrahimatix)&nbsp;&nbsp;
[![](https://img.shields.io/badge/Sponsor-GitHub-green?style=plastic&logo=github)](https://github.com/sponsors/ibrahimatix)&nbsp;&nbsp;


howtofindbugs is a simple Bash recon script that will simultaneously execute various subdomain enumeration tools, aggregate the results, and write entries to a file free of duplicates and then finally scan for low hanging bugs using projectdiscovery nuclei. This helps prevent discrepancies in enumeration tools, even those claiming to use similar sources. 

**Tools used:**
* [SubScraper](https://github.com/m8r0wn/subscraper)
* [Sublist3r](https://github.com/aboul3la/Sublist3r)
* [AssetFinder](https://github.com/tomnomnom/assetfinder)
* [Nuclei](https://github.com/projectdiscovery/nuclei)

### Install
Written for Debian-based Linux distributions (*Kali*, *Parrot Sec* & *Ubuntu*):

```text
git clone https://github.com/ibrahimatix/howtofindbugs.git
cd subwalker; chmod +x install.sh howtofindbugs.sh
sudo ./install.sh
```

### Usage
```text
#> ./howtofindbugs.sh example.com
[*] Executing SubWalker against: example.com
[*] Launching SubScraper
[*] Launching Sublist3r
[*] Launching assetfinder
[*] Waiting until all scripts complete...

[+] SubWalker complete with 107 results
[+] Output saved to: /opt/subwalker/howtofindbugs.txt

[*] Launching nuclei
```



