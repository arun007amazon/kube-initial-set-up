# kube-initial-set-up

## Initial Set Up:

### Enable 'Kubectl' for user:

Copy kube config to the user directory and set KUBECONFIG variable for the user.
`sudo cp /etc/kubernetes/admin.conf $HOME/` </br>
`sudo chown $(id -u):$(id -g) $HOME/admin.conf` </br>
`export KUBECONFIG=$HOME/admin.conf` </br>

Set KUBECONFIG during login:
	Edit path.sh in /etc/profile.d
	`sudo /etc/profile.d` </br>
	`export KUBECONFIG=$HOME/admin.conf`
