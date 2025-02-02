type:: [[town]]
icon:: 🏙️
domain:: [[Great Kingdom Neverwinter]] 
status::

- Details of this city:
	- Hatte mal eine Burg, ist aber nicht mehr besiedelt.
	- Generell hat das Dorf schon bessere Zeiten gesehen
- ![DALL·E 2025-01-23 22.05.56 - A detailed fantasy city map set in a hilly, alpine surrounding, featuring a smaller town with fewer buildings. The town is centered around a modest ma.jpg](../assets/DALL·E_2025-01-23_22.05.56_-_A_detailed_fantasy_city_map_set_in_a_hilly,_alpine_surrounding,_featuring_a_smaller_town_with_fewer_buildings._The_town_is_centered_around_a_modest_ma_1737666413718_0.jpg)
-
- query-table:: true
  query-properties::
  query-properties:: [:icon :page :description]
  #+BEGIN_QUERY
   {:title [:b "NPCs"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "[[Nethercrag]]")
  (property ?b :type "NPC")
   ]}
  #+END_QUERY
- query-table:: true
  query-properties:: [:icon :page :description]
  #+BEGIN_QUERY
   {:title [:b "Taverns"]
   :query [:find (pull ?b [*])   
   :where
  (property ?b :in "Nethercrag")
  (property ?b :type "Tavern")
   ]}
  #+END_QUERY