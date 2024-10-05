type:: [[town]]
icon:: 🏙️
domain:: [[Great Kingdom Neverwinter]]

- Große Stadt an der [[Hammersea]]
- Hauptstadt von [[Great Kingdom Neverwinter]]
- NPCs
	- query-sort-by:: block
	  query-table:: true
	  query-sort-desc:: true
	  query-properties:: [:description :block :page]
	  #+BEGIN_QUERY
	   {:title [:b "NPCs"]
	   :query [:find (pull ?b [*])   
	   :where
	  (property ?b :in "Neverwinter")
	  (property ?b :type "NPC")
	   ]}
	  #+END_QUERY
		- query-table:: false
		  #+BEGIN_QUERY
		  {
		    :title [:b "NPCs in Neverwinter (Page and Description)"]
		    :query [
		      :find (pull ?b [block/page])
		      :where
		        (property ?b :in "Neverwinter")
		        (property ?b :type "NPC")
		    ]
		  }
		  #+END_QUERY
			-
			- ock/p
- Taverns
	- {{query (and (property :in [[Neverwinter]]) (property :type [[Tavern]] ))}}
	  query-table:: true
	-
- ![neverwinter.png](../assets/neverwinter_1728047649096_0.png)