# Project 9 - Honeypot

Time spent: **4** hours spent in total

> Objective: Setup a honeypot and intercept some attempted attacks in the wild.

## Honeypots

1. dionaea
2. p0f
3. cowrie


## Issues
I used my own VPS to create instances of virtual machines for the MHN Admin Application and Honeypots. I was able to set up
the MHN Admin Application without any issues. However, when I set up the honeypot on another instance I was not able to get the
honeypot software running. The ports would be listed as closed. I attempted (for a very long time) to open the ports but when I ran
the wget command and tested used nmap, it would show that the ports are closed. Since the ports were closed I was not able to attack / or was
receiving any attacks.

I finally gave up and created all my honeypots in Google Cloud. My main admin application is still running from my server however.

## Data
- 165 total attacks for 1 hour combined
- TOP 5 Attacker IPs:
  1. 104.248.6.137 (7 attacks) - US
  2. 162.243.160.49 (7 attacks) - US
  3. 209.97.142.149 (6 attacks) - GB
  4. 188.166.3.86 (6 attacks) - NL
  5. 159.65.225.115 (5 attacks) - US

- TOP 5 Attacked Ports:
  1. 8088 (45 times)
  2. 23 (17 times)
  3. 445 (6 times)
  4. 81 (6 times)
  5. 5555 (5 times)

- Attacks by Honeypot
  1. dionaea - 117
  2. p0f - 48
  3. cowrie - 0

## Notes
I was disappointed that I was not able to get everything running from my own server.
