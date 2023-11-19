# Too many files error

sudo sysctl fs.inotify.max_user_instances=1280  
sudo sysctl fs.inotify.max_user_watches=655360

or permament editing /etc/sysctl.con using command  
fs.inotify.max_user_instances=1280  
fs.inotify.max_user_watches=655360


sudo sh -c 'echo "fs.inotify.max_user_instances=1280" >> /etc/sysctl.conf' && sudo sysctl -p   
sudo sh -c 'echo "fs.inotify.max_user_watches=655360" >> /etc/sysctl.conf' && sudo sysctl -p

sudo snap alias microk8s.kubectl kubectl

addons needed for microk8s 
dns
metallb