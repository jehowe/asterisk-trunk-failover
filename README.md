# asterisk-trunk-failover by Jeff Howe
Automation of outgoing trunk failover routing.

This code is ONLY part of the extensions.conf file and intended to provide a failover method
for outgoing calls where SIP provider redundancy is present (you have more than one SIP provider setup
in sip.conf).  If an outbound failure occurs (trunk unreachable, channel busy, etc), the outbound call is then tried on the second trunk, cycling through all the trunks until a call is successful.
