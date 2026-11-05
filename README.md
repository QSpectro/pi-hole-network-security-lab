# Pi-hole Network Security Lab

## Project Overview

This project documents my home lab using Pi-hole on a Raspberry Pi running Raspberry Pi OS. The goal is to demonstrate practical knowledge of DNS filtering, Linux administration, network services, and defensive network security.

## Project Goals

- Understand DNS resolution and how clients use DNS servers.
- Explore DNS-based filtering of unwanted domains.
- Practice Linux system administration on a Raspberry Pi.
- Document configuration, testing, and troubleshooting.
- Understand the security benefits and limitations of DNS filtering.

## Hardware and Software

| Component | Details |
|---|---|
| Hardware | Raspberry Pi 2 Model B |
| Operating system | Raspberry Pi OS Lite |
| DNS filtering software | Pi-hole |
| Pi-hole version | 6.5 |
| Network | Home network |
| DNS configuration | Router forwards DNS requests to Pi-hole |
| Administration | SSH / terminal |

## Network Architecture

Pi-hole provides DNS-based filtering for clients configured to use it as their DNS server.

The exact network design, client configuration, and DNS forwarding setup will be documented after verification.

## Implementation 

Pi-hole is installed and operational on a Raspberry Pi 2 Model B running Raspberry Pi OS Lite.

- **Pi-hole version:** 6.5
- **Blocking status:** Enabled
- **Network configuration:** Home router forwards DNS requests to Pi-hole
- **Administration:** SSH / terminal

## Initial Verification

The `pihole status` command confirmed that Pi-hole blocking is enabled.

This verifies that the blocking functionality is active, but additional testing is needed to confirm that DNS filtering is working as expected for client devices.


## Testing and Results

## DNS Resolution Testing

### Test 1: Successful DNS Resolution

**Command used:**

```bash
nslookup example.com 127.0.0.1
```

**Test Results:**
- DNS server responded successfully.
- DNS server address was displayed.
- The domain example.com resolved to IP addresses.
- DNS resolution through the local Pi-hole service was successful.

**Result:** PASS

**Skills Demonstrated:**
- DNS troubleshooting
- Linux command-line administration
- DNS server verification
- Network diagnostics


## Security Considerations

- DNS filtering is one layer of defense, not a replacement for firewalls or endpoint security.
- Administrative interfaces should be protected with strong credentials.
- Router and DNS settings should be changed carefully to avoid disrupting network connectivity.
- Credentials, private keys, and sensitive network information must not be committed to this repository.

## Skills Demonstrated

- DNS fundamentals
- Linux administration
- Raspberry Pi system management
- Network configuration
- Defensive security concepts
- Technical documentation

## Lessons Learned

I will document the concepts learned, configuration decisions, troubleshooting steps, and testing results as this project develops.

## Future Improvements

- Add a network architecture diagram.
- Document DNS resolution and filtering tests.
- Capture sanitized dashboard screenshots.
- Explore network monitoring and log analysis.
- Document backup and recovery considerations.

## References

- [Official Pi-hole Documentation](https://docs.pi-hole.net/)
- [Pi-hole GitHub Repository](https://github.com/pi-hole/pi-hole)
