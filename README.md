# F5 SSL Orchestrator SNI Library iRule
A PROC iRule function to retrieve the Server Name Indication (SNI) value from TLS Client Hello.

[![Releases](https://img.shields.io/github/v/release/kevingstewart/sslo-sni-library-rule.svg)](https://github.com/kevingstewart/sslo-sni-library-rule/releases)

### Version support
This utility works on BIG-IP 14.1 and above, SSL Orchestrator 5.x and above.

### How to install 
- Download the iRule to the F5 BIG-IP:

  ``echo -e "ltm rule /Common/library-rule {\n`curl -k https://raw.githubusercontent.com/kevingstewart/sslo-sni-library-rule/main/library-rule.tcl`\n}" > /var/tmp/library-rule & tmsh load sys config merge file /var/tmp/library-rule``


