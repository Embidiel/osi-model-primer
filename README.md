
# OSI Model

## Ano?

Ang ***OSI Model or Open Systems Interconnection (OSI)*** ay isang framework na kung saan ***pinapakita kung paano ba nakakapag-communicate ang different applications at networks*** by breaking down yung process into ***different layers.***

Ang OSI Model ay may ***7 different layers*** na kung saan nakakatulong
para sa isang engineer to identify yung cause ng problem sa network
kung meron man.

![enter image description here](https://res.cloudinary.com/practicaldev/image/fetch/s--jmQCnO87--/c_limit,f_auto,fl_progressive,q_auto,w_880/https://dev-to-uploads.s3.amazonaws.com/i/tt6b2sau1mdcg73qt4iz.png)

![enter image description here](https://imgur.com/9Ia0oqq.png)

## Layer 7 (Application Layer)

Dito nangyayari yung first step, sa browser. Kapag mag re-request ka ng data galing sa ibang server. Lahat ng data nandyan request body, headers, content type and etc.

## Layer 6 (Presentation Layer)
Optional layer. Dito tinatranslate na yung data mo in a format na maiintindihan nung server na kung saan ka nagre-request. 
Dito rin nagaganap yung encryption ng data mo using SSL kung naka https ka.

## Layer 5 (Session Layer)
Yung pag tag ng session between two computers or servers ay nangyayari dito. ***Nagkakaroon ng session id na auto generated or tag.***

## Layer 4 (Transport Layer)
Dito parang hinahati na yung data mo into `segments` that contains
source port number, destination port number, and sequence number.

Ineensure din nito na walang loss or damage yung data na ma-sesend sa next layer. Kapag nangyari yan magre-restart yung process from layer 7.

## Layer 3 (Network Layer)
Itong Network layer wala siyang alam sa mga port or laman nung data.
Ang alam niya lang ay may segment, tapos inaattach niya yung source ip address at destination ip address.

Yung segment ay magiging `packet` na this layer. Wala siyang pake kung may error or what basta se-send niya sa next layer.

## Layer 2 (Data Link Layer)

![enter image description here](https://res.cloudinary.com/practicaldev/image/fetch/s---yjj0kAu--/c_limit,f_auto,fl_progressive,q_auto,w_880/https://dev-to-uploads.s3.amazonaws.com/i/b5ei5bvi5duzzr2pgrc5.png)

Dito naman nangyayari yung abstraction ng hardware details nung nagpapadala ng data para pag pinadala sa next layer wala ng pake yung layer na yun kung anong type ba ng device yung ginamit sa data.

Pag yung packet dumaan dito ina-assign yung MAC Address ng device mo sa bawat packet tapos nabubuo na ang mga `ethernet frame.`

## Layer 1 (Physical Layer)

Dito dumadaan na yung ethernet frames sa mga wires, cables or wifi (basta kung saan nagco-connect yung mga pc, lol).

Dito yung ethernet frames mo magiging bits (1,0) through network cables, tawag dito modulation.

![enter image description here](https://imgur.com/VNTsQCw.png)

![enter image description here](https://res.cloudinary.com/practicaldev/image/fetch/s--exAnpe7n--/c_limit,f_auto,fl_progressive,q_auto,w_880/https://dev-to-uploads.s3.amazonaws.com/i/g0zs09l4i6w1qfakhd7t.jpg)



