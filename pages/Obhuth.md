type:: [[town]]
icon:: 🏙️
domain:: [[Dwarfen Kingdom of Morvuth]]
status::

- Details of this city:
	-
- query-table:: true
  query-properties::
  query-properties:: [:icon :page :description]
  #+BEGIN_QUERY
   {:title [:b "NPCs"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "[[Obhuth]]")
  (property ?b :type "NPC")
   ]}
  #+END_QUERY
- query-table:: true
  query-properties:: [:icon :page :description]
  #+BEGIN_QUERY
   {:title [:b "Taverns"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "[[Obhuth]]")
  (property ?b :type "Tavern")
   ]}
  #+END_QUERY