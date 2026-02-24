# Proof Artifacts

Run date: 2026-02-24 22:38:26 +07:00

Fork URL: https://github.com/sigmalogistikutama-collab/intercom
Selected app profile id: readiness_pulse
Selected app label: Intercom Readiness Pulse
Selected naming mode: namespaced
Selected proof style: sidechannel_focus
Mutating command: sync_readiness_pulse_sigmalogistikutama_collab_intercom
Query command: peek_readiness_pulse_sigmalogistikutama_collab_intercom
Payout Trac address: trac1he92eudp9730m3sqgkgq8e2vswzjfenqvqnyajajr2wmced7r8fqzzwuaz

Rationale: This run differs by using readiness-pulse state flow with namespaced command pair and sidechannel-stats proof via SC-Bridge CLI.

## Files
- run.log: pear runtime startup capture (sanitized).
- run-screenshot.png: visual render of run.log.
- command-mapping.log: protocol mapTxCommand output for selected command pair.
- sidechannel-stats.log: runtime /sc_stats capture through SC-Bridge CLI cli_result.

## Commands used
- pear run . --peer-store-name proof-pulse --msb-store-name proof-pulse-msb --subnet-channel proof-readiness-pulse --dht-bootstrap 127.0.0.1:49737 --sidechannels proof-pulse-room
- pear run . --peer-store-name proof-pulse-bridge --msb-store-name proof-pulse-bridge-msb --subnet-channel proof-readiness-pulse --dht-bootstrap 127.0.0.1:49737 --sidechannels proof-pulse-room --sc-bridge 1 --sc-bridge-cli 1 --sc-bridge-token <redacted> --sc-bridge-port 49339
- {"type":"cli","command":"/sc_stats"}
