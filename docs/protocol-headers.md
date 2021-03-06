# Protocol Headers

The following was pulled from Scapy, notice the defaults.

## IP

version    : BitField             = (4)
ihl        : BitField             = (None)
tos        : XByteField           = (0)
len        : ShortField           = (None)
id         : ShortField           = (1)
flags      : FlagsField           = (0)
frag       : BitField             = (0)
ttl        : ByteField            = (64)
proto      : ByteEnumField        = (0)
chksum     : XShortField          = (None)
src        : Emph                 = (None)
dst        : Emph                 = ('127.0.0.1')
options    : PacketListField      = ([])


## TCP

sport      : ShortEnumField       = (20)
dport      : ShortEnumField       = (80)
seq        : IntField             = (0)
ack        : IntField             = (0)
dataofs    : BitField             = (None)
reserved   : BitField             = (0)
flags      : FlagsField           = (2)
window     : ShortField           = (8192)
chksum     : XShortField          = (None)
urgptr     : ShortField           = (0)
options    : TCPOptionsField      = ({})


## DNS

id         : ShortField           = (0)
qr         : BitField             = (0)
opcode     : BitEnumField         = (0)
aa         : BitField             = (0)
tc         : BitField             = (0)
rd         : BitField             = (0)
ra         : BitField             = (0)
z          : BitField             = (0)
ad         : BitField             = (0)
cd         : BitField             = (0)
rcode      : BitEnumField         = (0)
qdcount    : DNSRRCountField      = (None)
ancount    : DNSRRCountField      = (None)
nscount    : DNSRRCountField      = (None)
arcount    : DNSRRCountField      = (None)
qd         : DNSQRField           = (None)
an         : DNSRRField           = (None)
ns         : DNSRRField           = (None)
ar         : DNSRRField           = (None)

