type:: [[town]]
icon:: 🏙️
domain:: [[Great Kingdom Neverwinter]]

- Große Stadt an der [[Hammersea]]
- Hauptstadt von [[Great Kingdom Neverwinter]]
- NPCs
	- {{query (and (property :in [[Neverwinter]]) (property :type [[NPC]]))}}
	  query-properties:: [:page :icon :description]
	  query-table:: true
	- query-sort-by:: block
	  query-table:: true
	  query-sort-desc:: true
	  query-properties:: [:page :description]
	  #+BEGIN_QUERY
	   {:title [:b "NPCs"]
	   :query [:find (pull ?b [*])   
	   :where
	  (property ?b :in "Neverwinter")
	  (property ?b :type "NPC")
	   ]}
	  #+END_QUERY
		-
		-
- Taverns
	- {{query (and (property :in [[Neverwinter]]) (property :type [[Tavern]] ))}}
	  query-table:: true
	-
- ![neverwinter.png](../assets/neverwinter_1728047649096_0.png)