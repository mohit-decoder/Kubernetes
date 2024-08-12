# COMMANDS TO EXECUTE: 
    kubectl apply -f deployment.yml
    kubectl rollout history deployment/myde
# kubectl annotate deployments.apps myde kubernetes.io/change-cause="Version-1" (Inperative Way Of Changeing Rollout History Change-Cause)
    kubectl rollout undo deployment/myde (Rollback Previous Version/Revision)
    kubectl rollout history deployment/myde --to-revision=5 (Rollback To Particular Version/Revision)
