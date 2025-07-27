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

POWERCOM_URL := https://www.upspowercom.com/pcm-img/Card-DA807/Upsmate_PCM.mib

all: XPPC-MIB

XPPC-MIB:
	@echo ">> Downloading XPPC-MIB"
	@curl $(CURL_OPTS) -o XPPC-MIB "$(POWERCOM_URL)"
	# Patch to replace RFC1213-MIB with SNMPv2-TC.
	@sed -i.bak -E 's/(DisplayString[[:space:]\n]+FROM) RFC1213-MIB/\1 SNMPv2-TC/' XPPC-MIB
	# Patch to fix malformed mib.
	@sed -i.bak2 -e 's/Normal(2}/normal(2) }/' -e 's/UPS Fault(/fault(/' XPPC-MIB
	@rm XPPC-MIB.bak XPPC-MIB.bak2

.PHONY: clean
clean:
	rm -rvf XPPC-MIB
