# Nord VPN Setup:

```bash
sudo wget -qnc https://repo.nordvpn.com/deb/nordvpn/debian/pool/main/nordvpn-release_1.0.0_all.deb;
sudo dpkg -i nordvpn-release_1.0.0_all.deb;
sudo apt update;
sudo apt install nordvpn;
```

Then, the following is exposed:

`nordvpn login` and then `nordvpn connect`
