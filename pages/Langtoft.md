type:: [[town]]
icon:: 🏙️
domain:: any

- Details of this city:
	-
- query-table:: true
  query-properties:: [:icon :page :description]
  #+BEGIN_QUERY
   {:title [:b "NPCs"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "Langtoft")
  (property ?b :type "NPC")
   ]}
  #+END_QUERY
- query-table:: true
  query-properties:: [:icon :page :description]
  #+BEGIN_QUERY
   {:title [:b "Taverns"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "Langtoft")
  (property ?b :type "Tavern")
   ]}
  #+END_QUERY
- ![langtoft.png](../assets/langtoft_1728035953167_0.png){:height 786, :width 748}
	- #