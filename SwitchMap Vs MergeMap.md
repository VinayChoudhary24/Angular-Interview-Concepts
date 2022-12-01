# switchMap Vs MergeMap

  **MergeMap
    --When we Want to Process All the Requests, we use MergeMap.
                 <!-- Example-- SEARCH BAR, where User wants to search Something-->
    --will always process all requests one by one.


  **SwitchMap
    --When we want to Process Only the Last Request, we Use SwitchMap.
                 <!-- Example-- SEARCH BAR, where User wants to search Something-->
    --Will Cancel the Previous requests and process the Last Request.