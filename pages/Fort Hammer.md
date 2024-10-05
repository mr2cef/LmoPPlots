type:: [[town]]
icon:: 🏙️
domain:: [[Great Kingdom Neverwinter]]

- Details of this city:
	-
- query-table:: true
  query-properties:: 
  query-properties::
  #+BEGIN_QUERY
   {:title [:b "NPCs"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "Fort Hammer")
  (property ?b :type "NPC")
   ]}
  #+END_QUERY
- query-table:: true
  query-properties:: [:icon :page :description]
  #+BEGIN_QUERY
   {:title [:b "Taverns"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "Fort Hammer")
  (property ?b :type "taver")
   ]}
  #+END_QUERY
- ![Fort Hammer2.jpg](../assets/Fort_Hammer2_1728035976375_0.jpg)