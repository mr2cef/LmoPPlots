type:: [[town]]
icon:: 🏙️
domain:: [[Great Kingdom Neverwinter]]

- Große Stadt an der [[Hammersea]]
- Hauptstadt von [[Great Kingdom Neverwinter]]
- NPCs
	- {{query (and (property :in [[Neverwinter]]) (property :type [[NPC]]))}}
	  query-properties:: [:page :icon :description]
	  query-table:: true
	- #+BEGIN_QUERY
	  {
	    :title "NPCs in Neverwinter (Sorted by Page Name)"
	    :query [
	      :find (pull ?b [*])
	      :where
	        [?b :block/properties ?p]
	        [(get ?p :in) [[Neverwinter]]]
	        [(get ?p :type) [[NPC]]]
	        [?b :block/page ?page]
	        [?page :block/name ?page-name]
	      ]
	    :result-transform (fn [result] (sort-by (fn [r] (get-in r [:block/page :block/name])) result))
	  }
	  #+END_QUERY
- Taverns
	- {{query (and (property :in [[Neverwinter]]) (property :type [[Tavern]] ))}}
	  query-table:: true
	-
- ![neverwinter.png](../assets/neverwinter_1728047649096_0.png)