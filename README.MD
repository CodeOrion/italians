`https://github.com/robertBrem/Microservices_with_Kubernetes`

Installiere mit Ansible: `ansible-playbook playbook.yml `

```
35.180.136.18
35.180.134.165
52.47.80.39
35.180.65.197
```

```
alias kc='kubectl --kubeconfig /home/vagrant/Schreibtisch/admin.conf'
alias wkc='watch kubectl --kubeconfig /home/vagrant/Schreibtisch/admin.conf'
kc get no
kc apply -f deployment.yml
kc delete -f deployment.yml
```

Zeige Pods: `kc get po`  
Zeige Services: `kc get svc`

`https://gist.github.com/robertBrem/ecfa00658c4951a098c44fb031804720`

`https://github.com/khinkali/semantic-releasing`

Jenkins: `http://35.180.136.18:30180/`  
Username: chopen  
Password: chopen  

Setup of Jenkins in Kubernetes
`kc create clusterrolebinding permissive-binding --clusterrole=cluster-admin --user=admin --user=kubelet --group=system:serviceaccounts`  
`https://illya-chekrygin.com/2017/08/26/configuring-certificates-for-jenkins-kubernetes-plugin-0-12/`  

Beispielapp: `https://github.com/khinkali/`