# Copyright The Prometheus Authors
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

include ../Makefile.curl

NET_SNMP_URL := https://raw.githubusercontent.com/net-snmp/net-snmp/v5.9/mibs

all: HCNUM-TC HOST-RESOURCES-MIB IF-MIB INET-ADDRESS-MIB IP-MIB IPV6-TC NET-SNMP-MIB NET-SNMP-TC SNMP-FRAMEWORK-MIB SNMPv2-MIB SNMPv2-SMI SNMPv2-TC UCD-SNMP-MIB

HCNUM-TC:
	@echo ">> Downloading HCNUM-TC"
	@curl $(CURL_OPTS) -o HCNUM-TC $(NET_SNMP_URL)/HCNUM-TC.txt

HOST-RESOURCES-MIB:
	@echo ">> Downloading HOST-RESOURCES-MIB"
	@curl $(CURL_OPTS) -o HOST-RESOURCES-MIB $(NET_SNMP_URL)/HOST-RESOURCES-MIB.txt

IF-MIB:
	@echo ">> Downloading IF-MIB"
	@curl $(CURL_OPTS) -o IF-MIB $(NET_SNMP_URL)/IF-MIB.txt

IP-MIB:
	@echo ">> Downloading IP-MIB"
	@curl $(CURL_OPTS) -o IP-MIB $(NET_SNMP_URL)/IP-MIB.txt

INET-ADDRESS-MIB:
	@echo ">> Downloading INET-ADDRESS-MIB"
	@curl $(CURL_OPTS) -o INET-ADDRESS-MIB $(NET_SNMP_URL)/INET-ADDRESS-MIB.txt

IPV6-TC:
	@echo ">> Downloading IPV6-TC"
	@curl $(CURL_OPTS) -o IPV6-TC $(NET_SNMP_URL)/IPV6-TC.txt

NET-SNMP-MIB:
	@echo ">> Downloading NET-SNMP-MIB"
	@curl $(CURL_OPTS) -o NET-SNMP-MIB $(NET_SNMP_URL)/NET-SNMP-MIB.txt

NET-SNMP-TC:
	@echo ">> Downloading NET-SNMP-TC"
	@curl $(CURL_OPTS) -o NET-SNMP-TC $(NET_SNMP_URL)/NET-SNMP-TC.txt

SNMP-FRAMEWORK-MIB:
	@echo ">> Downloading SNMP-FRAMEWORK-MIB"
	@curl $(CURL_OPTS) -o SNMP-FRAMEWORK-MIB $(NET_SNMP_URL)/SNMP-FRAMEWORK-MIB.txt

SNMPv2-MIB:
	@echo ">> Downloading SNMPv2-MIB"
	@curl $(CURL_OPTS) -o SNMPv2-MIB $(NET_SNMP_URL)/SNMPv2-MIB.txt

SNMPv2-SMI:
	@echo ">> Downloading SNMPv2-SMI"
	@curl $(CURL_OPTS) -o SNMPv2-SMI $(NET_SNMP_URL)/SNMPv2-SMI.txt

SNMPv2-TC:
	@echo ">> Downloading SNMPv2-TC"
	@curl $(CURL_OPTS) -o SNMPv2-TC $(NET_SNMP_URL)/SNMPv2-TC.txt

UCD-SNMP-MIB:
	@echo ">> Downloading UCD-SNMP-MIB"
	@curl $(CURL_OPTS) -o UCD-SNMP-MIB $(NET_SNMP_URL)/UCD-SNMP-MIB.txt

.PHONY: clean
clean:
	rm -rvf HCNUM-TC HOST-RESOURCES-MIB IF-MIB INET-ADDRESS-MIB IP-MIB IPV6-TC NET-SNMP-MIB NET-SNMP-TC SNMP-FRAMEWORK-MIB SNMPv2-MIB SNMPv2-SMI SNMPv2-TC UCD-SNMP-MIB
