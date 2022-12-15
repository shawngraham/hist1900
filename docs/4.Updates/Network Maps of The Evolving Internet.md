Some of you might be interested in doing some network analysis on the actual topology of the internet. Here's how you could do that.

You'll need:

- [gephi](https://gephi.org)
- within gephi, go to 'tools' -> plugins, install 'geolayout' (restart gephi), then under 'tools' -> plugins, install 'map of countries' (restart gephi)
- on the command line, `pip install zstandard`

Identify the data you want from [https://networks.skewed.de/net/internet_top_pop](https://networks.skewed.de/net/internet_top_pop)

Let's say I want `Arpanet196912`, on the command line run:

`curl https://networks.skewed.de/net/internet_top_pop/files/Arpanet196912.xml.zst --output "arpa1969.graphml.zst"`

Notice that in the output file name, I changed the `xml` to `graphml`. Still the same data, just makes it clearer what we're dealing with (for Gephi's sake)

Unzip:

`unzstd arpa1969.graphml.zst`

Fire up gephi. Under 'open graph file', select the file you just unzipped, eg `arpa1969.graphml`. Gephi will say there are some errors; you can ignore these for now. (Or you could try downloading the relevant csv version of the file, and then open that in Gephi; the csv might possibly be easier for Gephi to open.)

In the overview tab, under layout, select the 'geolayout'. Change projection to 'Transverse Mercator. Untick 'center'.

Then, under layout select 'map of countries'. In the drop down for countries, select 'World' then select 'north america' under subregion. Change 'projection' to 'transverse mercator', since that's the same as in your network data. Leave scale at 1000. **Untick 'center**'.

Ta da! In this way, you end up with the network topology pinned (more-or-less) to the real-world geography. But remember the actual *physical route* data would take to get from one node to the next is not (cannot be?) represented. And as far as network analysis goes, it's the topology - the pattern of what is connected to what - that matters. Select a more recent network map. Load it into Gephi. Run some statistics like 'betweeness centrality' (ie, a node that lies along the most shortest paths between every pair of nodes in the network) or 'modularity', nodes that share a similar pattern of localized interconnectivity. What might these metrics imply for the robustness of the internet, or the power of the agencies that control them, or the way that information might propagate through them?

![[arpanet1969.png]] 

_The ARPANet in 1969_