exclude-from-graph-view:: true

-
- # NPC
  template:: NPC
  template-including-parent:: false
	- type:: [[NPC]]
	  in:: anywhere
	  icon:: 👤
	  description:: anything
	  status::
	- ### Traits:
		-
	- ### Motivation:
		-
- ## Town
- template:: town
  template-including-parent:: false
	- type:: [[town]]
	  icon:: 🏙️
	  domain:: any
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
	  (property ?b :in "<% current page %>")
	  (property ?b :type "NPC")
	   ]}
	  #+END_QUERY
	- query-table:: true
	  query-properties:: [:icon :page :description]
	  #+BEGIN_QUERY
	   {:title [:b "Taverns"]
	   :query [:find (pull ?b [*])   
	   :where
	  (property ?b :in "<% current page %>")
	  (property ?b :type "Tavern")
	   ]}
	  #+END_QUERY
- ## Place
- template:: place
  template-including-parent:: false
	- type:: [[Place]]
	  icon:: 🏰
	  description:: anything
	  status::
- ## Tavern
- template:: tavern
  template-including-parent:: false
	- type:: [[Tavern]]
	  icon:: 🍻
	  in:: anywhere
	  status::
- # Plot
- template:: plot
  template-including-parent:: false
	- type:: [[Plot]]
	  icon:: ✍️
	  status::
-
- ## Artefact
- template:: artefact
  template-including-parent:: false
	- type:: [[Artefakt]] 
	  icon:: 💍