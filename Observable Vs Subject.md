# Observable Vs Subject

  **Observables
  --In Observable we need a separate OBSERVER interface to feed an Observable i.e They Can be Providers Not Consumers.
             <!-- Example -->
             getObservableData() {
                let myObservables = new Observable<any>( (observer) => {
                    observer.next("Observable Data...")
                });
                <!-- we Need to SUBSCRIBE -->
                myObservable.subscribe( (data) => {
                    this.observableData = data;
                });
             }

  --Observables are UNICAST by default- Each Subscribed observer owns an independent execution of the observable.


  **Subject
  --Subject Implements Both the Observable and the OBSERVER interfaces i.e They can be Both Providers and Consumers.
             <!-- Example -->
             getSubjectData() {
                let mySubject = new Subject();
                <!-- We Need to Subscribe Before Getting Data For Subject -->
                mySubject.subscribe( (data: string) => {
                    this.subjectData = data;
                });
                mySubject.next("Subject Data...")
             }

  --Subjects are MULTI-CASTING- the Execution i Shared among multiple subscribers