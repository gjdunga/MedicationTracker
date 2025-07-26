MedicationTracker
=================

MedicationTracker is a HIPAA‑compliant Android application created to help users
manage and track their medications securely.  It leverages RxNorm lookup to
ensure medication names are spelled correctly and to identify new drugs as
they become available.  Doses can be scheduled with timers that track days,
hours, minutes and seconds, and each dose records the amount in grams (g),
milligrams (mg) or micrograms (µg).  Totals per medication can be
calculated over configurable date ranges.

Key features include:

* **Secure encryption:** The app stores all personal health information using
  AES‑256 encryption through SQLCipher.  Encryption keys are derived from a
  user‑supplied password and a device‑specific salt.  Sensitive data such as
  the password itself is never persisted, and optional biometric unlock is
  supported.
* **Alarms and reminders:** Users are notified when it is time to take a
  medication.  Alarms show the medication name and dose and provide actions
  for marking the dose as taken, skipped (with confirmation) or snoozed for
  a user‑defined interval.  Alarm sound and volume can be customised in the
  settings menu.
* **Dose units and reporting:** Doses can be entered in g, mg or µg.  The app
  aggregates total amounts taken per medication and can generate reports over
  selected date ranges.  Reports can be exported as PDF files, optionally
  protected with the same password used to encrypt the database.
* **Import/export:** Data can be exported to a password‑protected ZIP file
  containing the encrypted database, password hash and salt.  This file can
  later be imported on another device to restore the user’s data.  There is
  also a reset option to start with a fresh database and password.
* **Audit logging:** Every addition, deletion or modification of a medication
  or dose is recorded in an immutable log to aid in compliance and provide
  an audit trail.

This application was developed by **Gabriel Dungan** with the assistance of
AI as a product of **DunganSoft Technologies**.  The trademarks **GJDUNGA**
and **DSTAFTN** are reserved.
