# OpenVPN install

## Step1

```
wget https://raw.githubusercontent.com/ltkal/QiXi-dn42-network-configfile/main/openvpn/openvpn-install.sh -O openvpn-install.sh
```
## Step2

```
chmod -v +x openvpn-install.sh
```

## Step3

```
sudo bash openvpn-install.sh
```

## Step4

```
sudo systemctl restart openvpn@server
```

## Step5

```
sudo apt purge openvpn
```

```
rm -rf /etc/openvpn
```
