# EC2 Connection Issues Troubleshooting

This lab covers scenarios where an EC2 instance becomes unreachable through SSH or RDP.

## Common Symptoms
- SSH connection times out
- RDP fails to connect
- Instance reachable from internal network only

## Tools Used
- AWS Console
- AWS CLI
- VPC Flow Logs
- Security Groups & Network ACLs

## Example Checks
1. Verify Security Group inbound rules (SSH/RDP from your IP).
2. Check NACL rules for ephemeral port ranges.
3. Confirm correct route table (public subnet → Internet Gateway).
4. Review VPC Flow Logs for REJECT traffic.
