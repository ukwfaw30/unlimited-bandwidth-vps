# Unlimited Bandwidth VPS: What Actually Gets Capped, Which Port Speed You Need, and What It Costs (JustHost Plans and Prices Compared)

JustHost's unmetered VPS starts at **$1.77/month** when you pay for 12 months, and the plan most buyers should take is **Vega**: 2 vCPU, 4 GB RAM, 80 GB NVMe and a 500 Mbit unmetered port for **$6.23/month** on annual billing ($7.79 month to month). No plan in the line has a monthly terabyte quota. What each one does have is a port speed, printed on the same line as the word UNMETERED, and that number is the real ceiling.

Below are all the unlimited-traffic plans JustHost lists on its VPS tariff page, what the port speeds work out to in terabytes per month, what the "fair-share" label in the spec means, and how a competitor's Asia-Pacific footnote shows what a genuine hidden quota looks like when a host leaves it off the plan card.

> **Quick pick.** Vega at $6.23/month on annual billing. 500 Mbit is about 155 TB a month, which covers a busy site, a VPN for a small team, or a mid-size download mirror. Running only a blog or an API? New Star at $1.77 is enough. Pushing video or disk images? Capella at $8.49 doubles nothing but the port, to 750 Mbit, for $2.26 more.
> 👉 [See JustHost's unmetered VPS plans and current prices](https://justhost.asia/en/services/vps/tariffs?ref=196392)

## Every JustHost unmetered VPS plan, side by side

All prices are US dollars. The first figure is the monthly rate; the second is the 20% discount JustHost applies when you pay for 12 months. The last column shows the traffic a port running flat out for 30 days would move, as JustHost itself states it.

| Plan | vCPU · RAM | NVMe | Unmetered port (≈ monthly ceiling) | Price: monthly / 12-month | Order |
| --- | --- | --- | --- | --- | --- |
| New Star | 1 · 1 GB | 10 GB | 100 Mbit (31+ TB) | $2.21 / **$1.77** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Sirius | 1 · 1 GB | 20 GB | 300 Mbit (93+ TB) | $2.81 / **$2.25** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Arcturus | 1 · 2 GB | 30 GB | 300 Mbit (93+ TB) | $4.01 / **$3.21** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Double Star | 2 · 2 GB | 20 GB | 200 Mbit (62+ TB) | $4.11 / **$3.28** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Alpha Centauri | 2 · 2 GB | 40 GB | 400 Mbit (124+ TB) | $5.21 / **$4.17** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Bright Star | 4 · 4 GB | 30 GB | 300 Mbit (93+ TB) | $5.68 / **$4.54** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Vega | 2 · 4 GB | 80 GB | 500 Mbit (155+ TB) | $7.79 / **$6.23** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Capella | 4 · 4 GB | 120 GB | 750 Mbit (232+ TB) | $10.61 / **$8.49** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Rigel | 4 · 8 GB | 200 GB | 750 Mbit (232+ TB) | $16.20 / **$12.96** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Antares | 5 · 8 GB | 300 GB | 750 Mbit (232+ TB) | $19.20 / **$15.36** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Betelgeuse | 6 · 12 GB | 400 GB | 750 Mbit (232+ TB) | $26.40 / **$21.12** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |
| Altair | 8 · 24 GB | 600 GB | 750 Mbit (232+ TB) | $47.40 / **$37.92** | [ order](https://justhost.asia/en/services/vps/tariffs?ref=196392) |

Two things in that table matter more than the prices.

**The port stops at 750 Mbit.** Above Capella you are buying RAM and disk, not bandwidth. Rigel, Antares, Betelgeuse and Altair all sit on the same 750 Mbit port as the $8.49 plan. If traffic volume is your problem, the expensive rows don't solve it.

**New Star, Double Star and Bright Star carry a minimum order of three months.** That's stated on the plan cards. The rest can be ordered month to month, though you lose the 20% discount if you do.

JustHost also sells a second VPS line where you pick the disk type, and those plans are cheaper per gigabyte of RAM than the NVMe line above:

| Tier | vCPU · RAM · Disk | HDD | SSD | NVMe |
| --- | --- | --- | --- | --- |
| Start | 1 · 512 MB · 5 GB | $3.25 / **$2.60** | $3.90 / **$3.12** | $4.22 / **$3.38** |
| Standard | 2 · 2 GB · 25 GB | $11.00 / **$8.80** | $13.20 / **$10.56** | $14.30 / **$11.44** |
| Super | 4 · 4 GB · 50 GB | $22.00 / **$17.60** | $26.40 / **$21.12** | $28.60 / **$22.88** |

The catch with this line: the storage-selector section doesn't print a port speed next to each plan. Given how the rest of the price list is built, assume the port is part of what you're giving up for the lower price and confirm it before ordering. There's also a separate IPv6-only VPS line listed from $1.60, which is a different product from the dual-stack plans above.

## What "unlimited" actually limits on a VPS

Three things get capped in this market, and only one of them is usually called a cap.

**Regional quotas.** OVHcloud advertises "truly unmetered bandwidth" on its VPS range, then excludes its Asia-Pacific data centres in a footnote: Mumbai, Singapore and Sydney come with a fixed monthly quota, and once you exceed it the port is throttled to 10 Mbps. The two OVHcloud pages that describe this don't even agree on the numbers. Its unmetered VPS page states 1 TB for VPS-1 and VPS-2, 3 TB for VPS-3 and VPS-4, and 4 TB for VPS-5 and VPS-6. Its SSD VPS page states 500 GB for VPS-1, 1 TB for VPS-2 and VPS-3, and 3 TB for VPS-4. Whichever figure applies to the plan you pick, the outcome is the same: a hard ceiling, then 10 Mbps, which is slower than most home connections.

**Port speed.** This is JustHost's model, and it's the honest version of "unlimited". You can move as much data as the port allows and nothing is metered, but the port is the arithmetic limit. 300 Mbit sustained for 30 days is about 97 TB; JustHost quotes 93+ TB after overhead. 500 Mbit comes to roughly 162 TB, quoted as 155+. 750 Mbit comes to about 243 TB, quoted as 232+. The ceiling exists, it just isn't enforced by a counter. It's enforced by physics.

**Post-threshold throttling.** The OVHcloud example above is the extreme case. Some hosts instead slow you down after a "reasonable use" threshold that never appears in the plan table. JustHost doesn't publish a threshold like that on its VPS pages, and the port number makes one largely redundant, but if you plan to run BitTorrent, a public proxy or a streaming relay, read the terms of service before you pay, because acceptable-use rules are a separate document from the bandwidth spec.

One more label worth decoding: every port in JustHost's table is marked **fair-share**. That means the port is shared with other VPS on the same machine. You're buying a share of 300, 500 or 750 Mbit, not a dedicated line, so a neighbour pulling hard can affect what you see in a speed test. For a website or a VPN this rarely shows. For anything where a sustained rate is contractual, budget for less than the headline figure.

> The useful question isn't "is it really unlimited" but "what happens at 3 a.m. on the worst day of the month". On a metered plan you get a bill or a suspension. On JustHost's model you get a slower port. On OVHcloud's Asia-Pacific plans you get 10 Mbps.
> 👉 [Compare JustHost's port speeds and 12-month prices](https://justhost.asia/en/vps?ref=196392)

## Which plan fits which job

**A blog, a brochure site, an API backend.** New Star at $1.77. 100 Mbit serves a few hundred thousand page views a month without strain, and 10 GB of NVMe holds a WordPress install with room to spare. Move up to Sirius at $2.25 if you want 20 GB of disk and a 300 Mbit port for 48 cents more.

**A VPN or proxy for a handful of people.** Port speed sets your ceiling here, because a single stream can eat a large share of a small port. Vega at 500 Mbit and $6.23 is the sensible floor; Sirius at 300 Mbit works for two or three users. Don't buy Altair for a VPN. It has 24 GB of RAM you'll never touch and the same 750 Mbit port as Capella.

**Downloads, mirrors, video, game-server updates.** Capella at $8.49 buys the top port for the least money, and 120 GB of NVMe. If the files themselves are large, the disk becomes the binding constraint before the port does: Rigel at $12.96 has 200 GB, Antares at $15.36 has 300 GB.

**Game servers and anything latency-sensitive.** Bandwidth is rarely the problem; distance is. A 750 Mbit port in the wrong country loses to a 300 Mbit port next to your players. JustHost's plan cards don't spell out data-centre locations, so confirm the location before you order, and check whether you can change it later if your players move.

**Anything that needs Windows.** The VPS pages describe KVM virtualisation and root access but don't list supported operating systems in the material I checked. Ask support before you pay for a year, and get the answer in writing.

## How JustHost compares with OVHcloud and KernelHost

Both competitors below are included for reference only. Currencies differ and no exchange rate is applied, so compare the shape of each offer, not the digits.

|  | JustHost | OVHcloud (SSD VPS) | KernelHost (Tokyo) |
| --- | --- | --- | --- |
| Cheapest plan | $1.77/mo, 12-month | From $4.54/mo (VPS-1) | €31.99/mo (Edge KVM-1) |
| Currency and billing | USD, 20% off with annual prepay | USD, "from" pricing | EUR, prepaid, no contract |
| Top port in the line | 750 Mbit | 500 Mbps to 3 Gbps depending on plan | Up to 1 Gbps on Edge, 500 Mbit to 3 Gbit on the classic line |
| Traffic model | Unmetered port, fair-share, no TB quota | Unmetered, except Asia-Pacific | No monthly quota, no per-TB charge, no throttle |
| Location exceptions | Not stated on plan cards | Mumbai, Singapore, Sydney: monthly quota then 10 Mbps | Tokyo unlimited plans carry a location surcharge, shown at checkout |

The OVHcloud column is the cautionary one. Its entry price is higher than JustHost's and its bandwidth story is cleaner on paper, right up until you order a Singapore VPS and hit the footnote. KernelHost sits at the other end: a European provider with a Tokyo presence, unmetered traffic at up to 1 Gbps, prepaid in euros with no minimum term, and an explicit surcharge for unlimited-bandwidth plans at that location. Its own documentation makes the point that actual speed depends on the route traffic takes, not on distance alone.

JustHost's position in that group is the cheap end of unmetered. $6.23 for 4 GB of RAM and a 500 Mbit port is not a price OVHcloud or KernelHost match on their published rates. What you give up for it is disclosure: the port is fair-share, the locations aren't on the plan cards, and the refund terms aren't stated on the pages I reviewed.

👉 [Check the current JustHost VPS lineup before prices change](https://justhost.asia/en/services/vps/tariffs?ref=196392)

## Before you pay for a year

Paying 12 months upfront is what unlocks the 20% discount, and it's also what makes a wrong choice expensive. Confirm these first:

1. **The port speed on the exact plan you're buying.** The storage-selector line doesn't show one.
2. **The data-centre location**, and whether it can be changed after delivery. KernelHost states plainly that its location is fixed once ordered; assume the same until JustHost says otherwise.
3. **IPv6.** JustHost sells dual-stack and IPv6-only VPS as separate lines, so check which one your plan belongs to.
4. **Windows support**, if you need it.
5. **The refund window.** It isn't on the VPS pages, and a 12-month prepay without a stated refund policy is a bet, not a purchase.
6. **The acceptable-use rules** if your workload is proxying, torrenting or media distribution.

If you only need a small site or an API endpoint, none of this is worth more than five minutes: New Star at $1.77 is cheap enough that a mistake costs less than lunch. If you're moving real traffic, Vega at $6.23 and Capella at $8.49 are the two plans where JustHost's price-per-megabit actually beats what the bigger names publish, and the 750 Mbit port on Capella is the highest throughput this lineup sells.

👉 [Start with JustHost's $1.77 plan or size up to a 750 Mbit port](https://justhost.asia/?ref=196392)
