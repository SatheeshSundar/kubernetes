# kubernetes files


Create cluster
kops create cluster --name=yourdomainname --state=s3://kops-state-du --zones=us-east-2a --node-count=2 --node-size=t2.micro --master-size=t2.micro --dns-zone=yourdomainname

Configure your cluster
kops update cluster --name yourdomainname --yes --state=s3://kops-state-du
