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
  (property ?b :in "Neverwinter")
  (property ?b :type "NPC")
   ]}
  #+END_QUERY
- query-table:: true
  query-properties:: [:icon :page :description]
  #+BEGIN_QUERY
   {:title [:b "Taverns"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "[[Neverwinter]]")
  (property ?b :type "NPC")
   ]}
  #+END_QUERY
- ![neverwinter.png](../assets/neverwinter_1728047649096_0.png)