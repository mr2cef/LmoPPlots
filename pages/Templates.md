# NPC
template:: NPC
template-including-parent:: false
	- type:: [[NPC]]
	  in:: anywhere
	  icon:: 👤
	  description:: anything
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
- ## Tavern
- template:: tavern
  template-including-parent:: false
	- type:: [[Tavern]]
	  icon:: 🍻
	  in:: anywhere
- # Plot
- template:: plot
  template-including-parent:: false
	- type:: [[Plot]]
	  icon:: ✍️
-
- ## Artefact
- template:: artefact
  template-including-parent:: fals
	- type:: [[Artefakt]] 
	  icon:: 💍