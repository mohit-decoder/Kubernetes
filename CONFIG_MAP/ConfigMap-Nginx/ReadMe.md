            kubectl create configmap default.conf --frome-file=default.conf
            kubectl create configmap default-conf --from-file=default.conf
            kubectl apply -f deployment.yml
            kubectl expose deployment newnginx --port 80 --target-port 9999 --type NodePort