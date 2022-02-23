# Launch instance in Public 1A
aws ec2 run-instances --image-id <value> --instance-type <value> --security-group-ids <value> --subnet-id <value> --key-name <value> --user-data <value>

# command
aws ec2 run-instances --image-id ami-033b95fb8079dc481 --instance-type t2.micro --security-group-ids sg-02cc4df3e66e3dfc3 --subnet-id subnet-02a3c09e42318c8e5 --key-name digital-cloud-labs-nv --user-data file://user-data-subnet-id.txt

# Launch instance in Public 1B
subnet-0dfd20b91d147dfca

aws ec2 run-instances --image-id ami-033b95fb8079dc481 --instance-type t2.micro --security-group-ids sg-02cc4df3e66e3dfc3 --subnet-id subnet-0dfd20b91d147dfca --key-name digital-cloud-labs-nv --user-data file://user-data-subnet-id.txt

# Launch instance in Private 1B
subnet-0fed8d0ccc6645a56

aws ec2 run-instances --image-id ami-033b95fb8079dc481 --instance-type t2.micro --security-group-ids sg-02cc4df3e66e3dfc3 --subnet-id subnet-0fed8d0ccc6645a56 --key-name digital-cloud-labs-nv --user-data file://user-data-subnet-id.txt


# Terminate instances

aws ec2 terminate-instances --instance-ids <value> <value>