# openvpn-k8s
image: lew21/openvpn-k8s

Install `vpn.yaml` with:
```
kubectl -n vpn create secret generic vpn-v1 --from-file=$DIR/../credentials/vpn/server.key --from-file=$DIR/../credentials/vpn/server.crt --from-file=$DIR/../credentials/vpn/dh.pem --from-file=$DIR/../credentials/vpn/client-ca.crt

```
