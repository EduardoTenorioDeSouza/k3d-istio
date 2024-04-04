# K3D com ISTIO

## Install current latest release
```
wget -q -O - https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash
```

```
curl -s https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash
```

## Quick Start k3d
```
k3d cluster create mycluster

kubectl get nodes
```

## Quick Start Istio
```
curl -L https://istio.io/downloadIstio | sh -
cd istio-1.21.0
export PATH=$PWD/bin:$PATH
```

## Install Istio
```
istioctl install
kubectl label namespace default istio-injection=enabled

```

# Referências

https://k3d.io/

https://istio.io/
