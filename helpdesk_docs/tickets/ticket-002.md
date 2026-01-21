# Ticket 002 — Websites Not Loading (DNS Error)

**User:** Angelys L.

## Issue
Unable to access websites due to a DNS configuration issue on the Ethernet adapter.
## Symptoms
- Browser displayed: DNS_PROBE_FINISHED_BAD_CONFIG
- Websites (example: speedtest.net) failed to load
- Network status showed Ethernet as connected with a valid IP address and default gateway
## Questions Asked
- Are you using a VPN or proxy connection?
- Is this the only website not working, or do other sites fail as well?
- Does the system show the network as connected?
## Troubleshooting Steps
- Opened Control Panel → Network and Internet → Network Connections to identify the active network adapter
- Reviewed proxy settings to confirm no manual proxy was enabled
- Checked IPv4 settings on the active Ethernet adapter
## Resolution
- Updated the DNS settings on the Ethernet adapter to use known, reliable DNS servers
- Flushed the DNS cache and reset the Windows network stack
- Restarted the system and verified that websites loaded successfully
## What I Learned
Even when a device shows it is connected to a network, incorrect DNS settings can prevent websites from loading. Using trusted DNS servers helps determine whether an issue is caused by local configuration problems or external network services
## Evidence
- [Browser DNS Error](../screenshots/ticket-002/01-dns-error-browser.png)
- [Ethernet Connected Status](../screenshots/ticket-002/02-ethernet-connected-status.png)
- [Proxy Settings](../screenshots/ticket-002/03-proxy-settings-off.png)
- [Active Network Adapter](../screenshots/ticket-002/04-active-network-adapter.png)
- [IPv4 DNS Settings](../screenshots/ticket-002/05-ipv4-dns-settings.png)
- [DNS Cache Flush](../screenshots/ticket-002/06-dns-cache-flush.png)
- [Winsock Reset](../screenshots/ticket-002/07-winsock-reset.png)
- [Website Verification](../screenshots/ticket-002/08-website-load-verification.png)

