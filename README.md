# snmp
Tools and configurations for translating SNMP into Prometheus

## Vendoring MIBs

This repo uses GNU make to automate vendoring MIB files.

For example, you can update the source URL in `<vendor>/Makefile` then run:

    make -C <vendor> clean
    make -C <vendor>
