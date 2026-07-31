# Cisco ISE Profiling Overview

## Overview

Cisco ISE Profiling automatically identifies endpoints connecting to the network and assigns them a profile based on collected attributes. This enables dynamic policy enforcement without manual endpoint classification.

## Profiling Sources

- DHCP
- RADIUS
- SNMP
- NetFlow
- HTTP
- DNS

## Profiling Workflow

1. Endpoint connects to the network.
2. ISE collects endpoint attributes.
3. Profiling policies evaluate the collected data.
4. The endpoint is assigned a profile.
5. Authorization policies apply the appropriate network access.

## Common Use Cases

- Corporate laptops
- IP phones
- Printers
- IoT devices
- Guest devices
- BYOD endpoints

## Verification Checklist

- Confirm profiling services are enabled.
- Verify endpoint attributes are being collected.
- Check assigned endpoint profiles.
- Validate authorization policy matches.
- Test endpoint access after profiling.

## Best Practices

- Enable only required probes.
- Review endpoint profiles regularly.
- Use descriptive profiling policies.
- Monitor profiling accuracy.
- Document profiling rules and exceptions.
