# TACACS+ Troubleshooting Guide

## Overview

This guide provides a structured approach to troubleshooting TACACS+ authentication, authorization, and accounting (AAA) issues in Cisco enterprise environments.

## Common Symptoms

- Unable to log in to network devices
- Authentication failures
- Authorization denied
- Command accounting not recorded
- Intermittent TACACS+ server connectivity

## Initial Checks

- Verify TACACS+ server reachability
- Confirm management interface connectivity
- Validate system time synchronization (NTP)
- Check TACACS+ service status

## Verification Commands

### Cisco IOS / IOS-XE

show aaa servers
show running-config | section aaa
show running-config | include tacacs
test aaa group tacacs+ <username> <password> legacy
show logging

## Common Root Causes

- Incorrect shared secret
- TACACS+ server unreachable
- ACL or firewall blocking TCP port 49
- Wrong source interface configured
- User not assigned the correct privilege level
- Clock synchronization issues

## Best Practices

- Configure redundant TACACS+ servers
- Use a dedicated management VRF where applicable
- Maintain local user accounts for emergency access
- Enable AAA accounting
- Monitor TACACS+ server health and authentication logs
