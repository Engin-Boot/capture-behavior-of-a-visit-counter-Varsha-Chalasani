# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given : Server stores the recent counter value in memory before shutdown
  And manual logging done in case of server failure.
  
  When : Server restarts.
  
  Then : Update the sensor counter.

Scenario: Reconcile counts if the sensor is offline for a while

  Given : Sensor can retrieve recent counter value
  And manual logging done when sensor goes offline.
  
  When : Sensor restarts.
  
  Then : Update sensor counter
