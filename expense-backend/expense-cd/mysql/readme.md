to use the ebs drivers I have refered to git hb repo and installed drviver 
kubectl apply -k "github.com/kubernetes-sigs/aws-ebs-csi-driver/deploy/kubernetes/overlays/stable/?ref=release-1.43"
and then after I have opened iam poliattached to nodes and add ebs policy to it..