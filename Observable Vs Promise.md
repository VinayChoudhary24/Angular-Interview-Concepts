# Observables Vs Promise

  **Observables
  --Observables have Three CALL BACKS--
                                  1- SUCCESS
                                  2- ERROR
                                  3- COMPLETE
  
  --Observables are LAZY-- Observables will not Execute Untill we SUBSCRIBE to Them.

  --Observables emits MULTIPLE Values over a period of time.
                 <!-- Example -->
                 observer.next("Observable has emitted 1");
                 observer.next("Observable has emitted 2");
                 observer.next("Observable has emitted 3");

 --Observables is CANCELLABLE i.e We can UNSUBSCRIBE to Them.

 --Observables Can be SYNCHRONOUS or ASYNCH.

 --Observables Also Supports Rxjs Operators like filter(), map(), reduce() etc.....


 **Promises
 --Promise have Two CALL BACKS--
                            1- SUCCESS
                            2- ERROR

 --Promises are NOT LAZY-- Prmoises Execute immediately once after it is created.

 --Promises emits only ONE Value at a Time.
                 <!-- Example -->
                 resolve("Promise has emitted 1");
                 resolve("Promise has emitted 2");
                 resolve("Promise has emitted 3");

 --Promise is NOT CANCELLABLE

 --Promises are Always ASYNCH.

 --Promises Does NOT Supports Rxjs Operators.