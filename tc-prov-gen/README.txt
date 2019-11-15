* e1.dlv: small example graph
* e2.dlv: a few extra edges (to be added to e1)

* tc4.dlv:
A set of rules to compute the transitive closure (tc/2) of the given graph/edge relation (e/2).
The original rules for tc are "rewritten" to create a version tc4 (since it's a 4-ary relation):
tc4(X,Y, IX,IY) means that in the given graph there is a path from X to Y and the edge (IX,IY) lies on some such path.

When invoking the DLV tool with tc4.dlv make sure to include e1.dlv (or e1.dlv + e2.dlv) on the command line!


* tc4p.dlv:
Now adding the "p" for Possible Worlds!
First, let's put some edges e/2 into this file directly (for simplicity.. so no separate {e1,e2}.dlv files...

But let's say we don't know the complete graph, i.e., there are some edges that may or may not be there.
For these I define a set of nodes n/1 such that pairs of edges between nodes can be invented.

See the comments in that file to find out how to invoke these rules and how to do some interesting analysis / post-processing...




