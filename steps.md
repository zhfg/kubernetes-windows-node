```
[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12
Start-BitsTransfer https://github.com/kubernetes-sigs/sig-windows-tools/archive/master.zip
tar -xvf .\master.zip --strip-components 3 sig-windows-tools-master/kubeadm/v1.15.0/*
Remove-Item .\master.zip
```
