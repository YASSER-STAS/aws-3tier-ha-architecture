# Network Design

## VPC

Name: aws-3tier-vpc

CIDR: 10.0.0.0/16

Region: eu-west-2 (London)

## Availability Zones

- eu-wset-2a
- eu-west-2b

## Subnet Plan

| Layer|   | Subnet|      | CIDR  |          |  AZ |

| Public  | Public-A    | 10.0.1.0/24    | eu-west-2a |
| Public  | Public-B    | 10.0.2.0/24    | eu-west-2b |
| App     | App-A       | 10.0.10.0/24   | eu-west-2a |
| App     | App-B       | 10.0.11.0/24   | eu-west-2b |
| Data    | Data-A      | 10.0.20.0/24   | eu-west-2a |
| Data    | Data-B      | 10.0.21.0/24   | eu-west-2b |