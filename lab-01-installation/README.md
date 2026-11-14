
# LAB 01 — Initial RHEL Server Configuration

## Objective
Configure and validate a Red Hat Enterprise Linux server.

## Environment
- OS: Red Hat Enterprise Linux 10.3
- Virtualization: VMware Workstation
- Installation: Minimal
- Administrator: adminlinux

## Tasks completed
1. Installed RHEL 10.3
2. Configured the hostname
3. Verified operating system information
4. Inspected network interfaces and routing
5. Verified administrator privileges

## Commands used

```bash
sudo hostnamectl set-hostname rhel-lab-01
hostnamectl
cat /etc/redhat-release
ip -br addr
ip route
id
sudo whoami
```

## Validation results
- Hostname: rhel-lab-01
- OS: RHEL 10.3
- Network interface: ens160 (UP)
- Network: 192.168.174.0/24 (VMware lab)
- Administrative group: wheel
- `sudo whoami` returned `root`

## Troubleshooting
Nano was initially unavailable on the minimal installation.

Solution:
```bash
sudo dnf install -y nano
```

## Skills demonstrated
- Linux server configuration
- Network inspection
- Privilege management with sudo
- Software installation with DNF
- Technical documentation
