<!-- Canonical version, kept up to date: https://cheap-intelligence.vercel.app/en/playbooks/chain-of-custody
     Generated from the Practicum. Do not edit here — edits are overwritten on the next release. -->

> **Draft translation, not author-reviewed.** The Russian edition is the source of truth.

# Chain of custody: the first day with an important file

> Practicum for **Volume 3, Chapter 10**. Time: 10 to 15 minutes.
> This is a practical first-preservation protocol, not digital forensics or legal advice.

An important file rarely loses a dispute because it looks unconvincing. The problem is often simpler. Nobody knows where the file came from, whether it changed, or who handled it. This worksheet helps you preserve your options. It cannot guarantee that a bank, newsroom, or court will accept the file, but it can stop you from destroying a useful trail yourself.

---

## Start with four actions

### 1. Save the original

- Take the source file from the device or service where it first appeared.
- Do not make a messenger copy your only copy. The service may compress the file or remove some metadata.
- Create a working copy. Store the original separately and do not edit it again.
- Preserve the nearby context: the conversation, email, call record, receipt, and login log.

**Path to the original:** ________________________________________________

### 2. Record who, when, and what

| Date and time | Who had the file | What they did | Recipient or storage location |
|---|---|---|---|
| | | | |
| | | | |
| | | | |

Fill in the log right away. You can add to your own log later, so the log alone proves nothing. Its value comes from links to independent records, such as an email, cloud version history, bank case number, or police report number.

### 3. Create an independent record of the file

Choose a method that matches the cost of a possible error:

- A **checksum** shows that two files match bit for bit. It does not identify the author or prove a date by itself.
- A **channel with an external timestamp**, such as a company system, cloud version history, or registered case, can help show that the file already existed at a certain time.
- A **specialist or notary** is useful when a dispute is already likely and the cost of an error is high, not simply "just in case."

**Checksum or external record:** __________________________________________

### 4. Do not improve the original

Noise reduction, upscaling, editing, and a command such as "make it clearer" create a derivative version. That version may be easier to inspect, but it is no longer identical to what the device recorded.

- Leave the original untouched.
- Give an enhanced or cropped version a different name.
- Record which tool created the derivative copy and why.

---

## During the first day

- [ ] Contact the bank on the same day if money is involved. Save the case number.
- [ ] Save the bank statement, receipt, and recipient details.
- [ ] Export the conversation or email with dates and technical headers when they are available.
- [ ] Record the names of people who witnessed the event or saw the file.
- [ ] Ask the employer, platform, or contractor to preserve system logs if they control them.
- [ ] If a dispute is likely, contact the right party: the bank and police for money or fraud, a lawyer for a contract or workplace issue, or a fact-checking desk for a publication.

## What usually weakens a file

- the only copy is a forwarded message or screenshot;
- renaming the file without recording its original name;
- editing the original;
- deleting nearby messages and notifications;
- waiting a long time before creating the first independent record;
- assuming that "the recording speaks for itself."

---

## Transfer record

Copy this block every time you transfer the file:

```text
File:
Original name:
When and where it appeared:
Received from:
Checksum:
Transferred to:
Date and method of transfer:
What was transferred: original / exact copy / derivative copy
Changes made:
Related independent record:
```

---

This protocol is based on [NIST SP 800-86](https://www.nist.gov/publications/guide-integrating-forensic-techniques-incident-response): record every action involving digital material, preserve the source, and verify integrity. NIST describes it as a practical guide to computer forensics, not legal instructions for every country.

*Related worksheets:* [Personal trust perimeter](trust-perimeter.md),
[Evidence package before a dispute](evidence-package.md), and
[Trust and the law](https://cheap-intelligence.vercel.app/en/watch/trust-regulation).
