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
	-
	- {{query (and (property :in <% current page %>) (property :type [[NPC]]))}}
	  query-table:: true
	  query-properties:: [:icon :page :description]
	- Taverns
		- {{query (and (property :in <% current page %>) (property :type [[Tavern]] ))}}
		  query-table:: true
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
-