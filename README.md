# howtofindbugs
[![](https://img.shields.io/twitter/follow/ibrahimatix0x01?color=blue&label=Twitter&logo=twitter&style=plastic)](https://twitter.com/ibrahimatix0x01)&nbsp;&nbsp;
[![](https://img.shields.io/github/followers/ibrahimatix0x01?color=gray&label=GitHub&logo=github&style=plastic)](https://github.com/ibrahimatix0x01)&nbsp;&nbsp;
[![](https://img.shields.io/badge/Sponsor-GitHub-green?style=plastic&logo=github)](https://github.com/sponsors/ibrahimatix0x01)&nbsp;&nbsp;


howtofindbugs is a simple Bash recon script that will simultaneously execute various subdomain enumeration tools, aggregate the results, and write entries to a file free of duplicates and then finally scan for low hanging bugs using projectdiscovery nuclei. This helps prevent discrepancies in enumeration tools, even those claiming to use similar sources. 

**Tools used:**
* [SubScraper](https://github.com/m8r0wn/subscraper)
* [Sublist3r](https://github.com/aboul3la/Sublist3r)
* [AssetFinder](https://github.com/tomnomnom/assetfinder)
* [Nuclei](https://github.com/projectdiscovery/nuclei)

### Install
Written for Debian-based Linux distributions (*Kali*, *Parrot Sec* & *Ubuntu*):

```text
git clone https://github.com/ibrahimatix0x01/howtofindbugs
cd howtofindbugs; chmod +x install.sh howtofindbugs.sh
sudo ./install.sh
```

### Usage
```text
#> ./howtofindbugs.sh example.com
[*] Executing HowToFindBugs against: example.com
[*] Launching SubScraper
[*] Launching Sublist3r
[*] Launching Assetfinder
[*] Waiting until all scripts complete...

[+] HowToFindBugs complete with 44results
[+] Output saved to: /opt/ibrahimatix/example.com/howtofindbugs.txt

[*] Launching nuclei
```

<a href="https://www.buymeacoffee.com/ibrahimatix" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>

