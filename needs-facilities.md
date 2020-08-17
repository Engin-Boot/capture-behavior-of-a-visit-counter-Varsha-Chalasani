# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given : Entry-card issuer type sensor, staff not called visitors,
  sensor differentiates among patients, relatives and visiting doctors.
  Reset counter everyday.
  When : visitor enters.
  Then : Separate counters maintained for different types of visitors.
  Categorize every entry and issue a card. Increment respective counter.
  Compute and present trends.

Scenario: Alert when seating capacity is full

  Given : Seating meant for visitors alone, entry-card issuer
  sensor type, visitors-exit log maintained.
  When : every 15 minutes.
  Then : increment visit-counter after an entry, decrement exit-counter
  after an exit, subtract both every 15 minutes and check with maximum
  seat capacity. If exceeds, trigger an alert.
