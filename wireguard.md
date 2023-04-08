# wireguard-install

## Step 1

```
install wireguard/wireguard-tools
```

## Step2

```
wg genkey | tee privatekey | wg pubkey > publickey
```

## Step3

```
[Interface]
ListenPort = 
PrivateKey = 
PostUp = /sbin/ip addr add dev %i /32 peer /32
PostUp = /sbin/ip addr add dev %i /128 peer /128
Table = off

[Peer]
Endpoint = 
PublicKey = 
AllowedIPs = 
PersistentKeepalive = 25

```

## Step4

```
wg-quick up x
```
