Internet
   ↓
ALB Security Group
vs-vpc-alb-sg allow HTTP from 0.0.0.0/0
   ↓
EC2 Security Group
vs-vpc-app-sg allow HTTP from vs-vpc-alb-sg
   ↓
RDS Security Group
vs-vpc-data-sg allow Mysql/Aurora from vs-vpc-app-sg