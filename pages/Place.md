icon:: 🌍️
exclude-from-graph-view:: false

- {{query (and (property :type [[Place]]) (not (page [[Templates]])))}}
  query-table:: true
  query-properties:: [:icon :description :page :in]
  query-sort-by:: page
  query-sort-desc:: false
