type:: [[town]]
icon:: 🏙️
domain:: [[Great Kingdom Neverwinter]]

- Große Stadt an der [[Hammersea]]
- Hauptstadt von [[Great Kingdom Neverwinter]]
- NPCs
	- {{query (and (property :in [[Neverwinter]]) (property :type [[NPC]]))}}
	  query-properties:: [:page :icon :description]
	  query-table:: true
		- query-table:: false
		  #+BEGIN_QUERY
		  {
		    :title "NPCs in Neverwinter"
		    :query [
		      :find (pull ?b [*])
		      :where
		        [?b :block/properties ?p]
		    ]
		  }
		  #+END_QUERY
			-
			-
- Taverns
	- {{query (and (property :in [[Neverwinter]]) (property :type [[Tavern]] ))}}
	  query-table:: true
	-
- ![neverwinter.png](../assets/neverwinter_1728047649096_0.png)