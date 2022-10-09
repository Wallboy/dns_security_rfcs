**NOTE:** *This repository is for informational and educational purposes only and shouldn't be taken as 100% accurate*

This repository contains an SVG graph that shows an (nearly) exhaustive list of DNS Security related RFCs grouped by subject such as: DNSSEC, DANE, DoT, DoH, etc as of October 2022. The RFCs are then sorted top down by release year (seen on the left). Each of the RFC Nodes has it's title as a Tooltip and clicking them bring you to the respective RFC.

### How the SVG was generated
The graph was created using this great RFC Dependancy Graphing tool: https://github.com/raybellis/rfcdeps

`./rfcdeps --no-older dns_security.cfg > raw_graph.gv`

*raw_graph.gv* was then manually edited to group/cluster RFCs into a relevant DNS Security category

`dot -Tsvg edited_graph.gv > dns_security_rfcs.svg`
