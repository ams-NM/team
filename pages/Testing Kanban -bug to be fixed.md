-
- Issue: [[Logseq]]'s newly added ==query-table::== breaks the logic of `Kanban` plugin
	- Ref: https://github.com/hkgnp/logseq-kanban-plugin/issues/25
- {{renderer :kanban_cyixdnuu}}
	- tasks
		- query-table:: false
		  #+BEGIN_QUERY
		  {
		   :query [
		           :find (pull ?b [*])
		           :where
		          [?b :block/page ?p]
		          (not (page-property ?p :type "templates"))
		          (task ?b #{"TODO" "DOING" "DONE"})
		           ] 
		   }
		  #+END_QUERY
- query-table:: false
  query-sort-by:: plan
  query-sort-desc:: false
- Experiments
	- Pending
		- ((64336b8e-cbbc-4936-9eaa-81319c456bda))
	- Planed
		- ((64336b8e-01de-4953-b9c0-3f9f716ca3d0))
	- Done
		- ((64336b8e-a294-4a9a-9e28-fea5c609236a))
	-
	-
-