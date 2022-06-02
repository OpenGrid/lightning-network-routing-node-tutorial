# lightning-network-routing-node-tutorial
Przewodnik po prowadzeniu węzła rutującego [sieci Lightning](https://lightning.network/)

1. [Budowanie płynności](#budowanie-płynności)
2. [Narzędzia](#narzędzia)

## Budowanie płynności

### Krok 1 - płynność wychodząca (outbound liquidity)
Otwierając kanał do innego węzła zwiększasz swoją płynność wychodzącą. Jest to ilość środków jakie jesteś w stanie przesłać dalej w płatnościach własnych lub gdy przekazujesz je od kogoś. Otwieranie kanałów warto rozpocząć od serwisów, z których sam korzystasz, takich jak portfele, giełdy, kopalnie, procesorzy płatności, znajome usługi, przyjaciele, etc. Zapewni Ci to szybsze i tańsze płatności do nich.
Przykładowo:

Serwis | Rodzaj | Węzeł
------|--------|------
[Bitrefill](https://www.bitrefill.com/lightning-toplist/?hl=en) | Karty podarunkowe |  https://www.bitrefill.com/lightning-toplist/?hl=en
[Tippin.me](https://tippin.me/) | Napiwki | https://1ml.com/node/03c2abfa93eacec04721c019644584424aab2ba4dff3ac9bdab4e9c97007491dda
[OpenNode](https://www.opennode.com/) | Operator płatności | https://1ml.com/node/03abf6f44c355dec0d5aa155bdbdd6e0c8fefe318eff402de65c6eb2e1be55dc3e
[Nicehash](https://www.nicehash.com/nicehash-lightning-network-node) | Mining pool | https://1ml.com/node/037659a0ac8eb3b8d0a720114efc861d3a940382dcfa1403746b4f8f6b2e8810ba
[BlueWallet](https://bluewallet.io/) | Portfel | https://lndhub.io/
[Wallet Of Satoshi](https://walletofsatoshi.com/) | Portfel | https://1ml.com/node/035e4ff418fc8b5554c5d9eea66396c227bd429a3251c8cbc711002ba215bfc226
[Remote Admin VPS](https://ln-vps.remoteadmin.store/) | Hosting | https://1ml.com/node/025033fdfd6f4e0e909776f0e8250c997f75de9cb11466e3a36fb8e6c7a1abcbb9

Ewentualnie możesz kierować się rankingiem BOS: https://cheeserobot.org/bos/list

### Krok 2 - płynność przychodząca (inbound liquidity)
Gdy ktoś otworzy kanał do Ciebie, zwiększa swoją płynność wychodzącą, ale i zwiększa Twoją płynność przychodzącą. To pozwala Ci przymować płatności, lub przekazywać cudze. Wskazówki:
* otwórz kanał o wielkości trochę ponad 0.00500000 BTC (500k sats) z [Lightning Conductor](https://lightningconductor.net/channels). Automatycznie otrzymasz kanał przychodzący o pojemności 0.00500000 BTC (500k sats)
* Jeżeli masz minimum 10 kanałów możesz skorzystać z usługi https://ln2me.com/ aby otrzymać równoważny kanał.

### Krok 3 - kręgi koordynowane
Dołączaj do kręgów koordynowanych na stronie [LightningNetwork+](https://lightningnetwork.plus/)

Najlepiej jak masz już minimum 10 kanałów i większą całkowitą pojemność kanałów. W ten sposób możesz zakwalifkować się do lepszych kręgów lub wymagać lepszych węzłów do udziału w Twoich kręgach.

### Krok 4 - kup kanały przychodzące
* [Zero Fee Routing](https://zerofeerouting.com/)
* [LND ⚡ Routing](https://github.com/lnd-routing/lnd-routing)
* [LNBIG](https://lnbig.com/#/open-channel)
* [Coincept](https://coincept.com/)
* [Yalls](https://yalls.org/about/)

## Narzędzia
W miarę budowania płynności i nawiązywania relacji możesz korzystać z następujących narzędzi by analizować swój węzeł, konkurencję (czyli poziomy opłat innych węzłów do tych samych destynacji), etc.
* [Terminal Web](https://terminal.lightning.engineering/)
* [lnchannels](https://ln.fiatjaf.com/)
* [Amboss Space](https://www.amboss.space/)
* [LNRouter](https://lnrouter.app/app/lookups)
* [LN Node Insight](https://lnnodeinsight.com)
* [1ml.com](https://1ml.com)
* [LightningNetwork+](https://lightningnetwork.plus/)

