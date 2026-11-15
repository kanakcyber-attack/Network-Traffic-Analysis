# Wireshark Display Filter Quick Reference

| Purpose | Display filter |
|---|---|
| ICMP | `icmp` |
| DNS | `dns` |
| TCP | `tcp` |
| UDP | `udp` |
| HTTP | `http` |
| TLS | `tls` |
| One IP address | `ip.addr == 192.0.2.10` |
| One TCP port | `tcp.port == 443` |
| Initial TCP SYN packets | `tcp.flags.syn == 1 && tcp.flags.ack == 0` |
| TCP retransmissions | `tcp.analysis.retransmission` |
| TCP resets | `tcp.flags.reset == 1` |
| DNS responses with errors | `dns.flags.rcode != 0` |
| HTTP POST requests | `http.request.method == "POST"` |

Replace example addresses with addresses from your authorized lab. These filters help narrow analysis; they do not establish malicious intent by themselves.
