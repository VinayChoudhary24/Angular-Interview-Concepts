# ngOnChanges Vs ngDoCheck

  **ngOnChanges
    --it is ONLY called when the CHILD component receives a value from PARENT using @Input decorator.
    --will be called when data bound input property changes.


  **ngDoCheck
    --will be called for every change detection.