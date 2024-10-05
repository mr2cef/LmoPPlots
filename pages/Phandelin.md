query-table:: true
query-properties:: [:page :icon :description]
type:: [[town]]
icon:: 🏙️
domain:: [[Great Kingdom Neverwinter]]

- Dorf, mit Abenteuer
- query-table:: true
  query-properties:: [:icon :page :description]
  #+BEGIN_QUERY
   {:title [:b "NPCs"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "Phandelin")
  (property ?b :type "NPC")
   ]}
  #+END_QUERY
-
- Taverns
	- {{query (and (property :in [[Phandelin]]) (property :type [[Tavern]] ))}}
	  query-table:: true