# lightning-network-routing-node-tutorial
Przewodnik po prowadzeniu węzła rutującego [sieci Lightning](https://lightning.network/)

1. [Budowanie płynności](#budowanie-płynności)
2. [Narzędzia](#narzędzia)

## Budowanie płynności

### Krok 1 - Serwisy, z których często korzystasz
Tacy jak: sprzedawcy, giełdy, kopalnie, procesorzy płatności, dobrzy znajomi, etc. Zapewni Ci to szybsze i tańsze płatności.
Przykładowo:
* [Bitrefill](https://www.bitrefill.com/lightning-toplist/?hl=en)
* [Tippin.me](https://1ml.com/node/03c2abfa93eacec04721c019644584424aab2ba4dff3ac9bdab4e9c97007491dda)
* [OpenNode](https://cheeserobot.org/node/03abf6f44c355dec0d5aa155bdbdd6e0c8fefe318eff402de65c6eb2e1be55dc3e)
* [Nicehash](https://www.nicehash.com/nicehash-lightning-network-node)
* [OpenNode](https://1ml.com/node/03abf6f44c355dec0d5aa155bdbdd6e0c8fefe318eff402de65c6eb2e1be55dc3e)
* [BlueWallet](https://lndhub.io/)
* [Remote Admin VPS](https://ln-vps.remoteadmin.store/)

Ewentualnie możesz kierować się rankingiem BOS: https://cheeserobot.org/bos/list

### Krok 2 - kanały zwrotne
Następnie otwórz kanał o wielkości trochę ponad 0.00500000 BTC (500k sats) z [Lightning Conductor](https://lightningconductor.net/channels). Automatycznie otrzymasz kanał przychodzący o pojemności 0.00500000 BTC (500k sats)

Jeżeli masz minimum 10 kanałów możesz skorzystać z usługi https://ln2me.com/ aby otrzymać równoważny kanał. 

### Krok 3 - kręgi koordynowane
Dołączaj do kręgów koordynowanych na stronie [LightningNetwork+](https://lightningnetwork.plus/)

Najlepiej jak masz już minimum 10 kanałów i większą całkowitą pojemność kanałów. W ten sposób możesz zakwalifkować się do lepszych kręgów lub wymagać lepszych węzłów do udziału w Twoich kręgach.

### Krok 4 - kup kanały przychodzące
* [LND ⚡ Routing](https://github.com/lnd-routing/lnd-routing)
* [LNBIG](https://lnbig.com/#/open-channel)
* [Coincept](https://coincept.com/)
* [Yalls](https://yalls.org/about/)

## Narzędzia
W miarę budowania płynności i nawiązywania relacji możesz korzystać z następujących narzędzi by analizować swój węzeł, konkurencję (czyli poziomy opłat innych węzłów do tych samych destynacji), etc.
* [Terminal Web](https://terminal.lightning.engineering/)
* [lnchannels](https://ln.fiatjaf.com/)
* [Amboss Space](https://www.amboss.space/)
