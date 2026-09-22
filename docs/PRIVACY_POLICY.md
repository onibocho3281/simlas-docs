# Simlas Privacy Policy

**Effective date:** September 22, 2026

Simlas is an unofficial Discord companion application for *The Witcher TRPG*. This Privacy Policy explains what information Simlas processes, why it is processed, and how users can request deletion of information associated with them.

## 1. Information Simlas processes

Depending on how Simlas is used, it may process and store:

- Discord user IDs and basic Discord account information needed to associate users with games and characters;
- Discord server, channel, and role-related identifiers needed to manage games, memberships, permissions, and bound channels;
- character references and metadata associated with C.O.D.I. character sheets;
- Google Sheets identifiers or references required to access C.O.D.I. sheets that users or game administrators deliberately make available to Simlas;
- game state such as encounters, initiative, turn state, conditions, combat transactions, equipment state, and other persistent gameplay records;
- command-related audit information and stored transaction identifiers used for replay safety, debugging, and game-state consistency.

Simlas may also receive information supplied directly through Discord commands and interactions.

## 2. Google Sheets and C.O.D.I.

Simlas uses a Google service account to access C.O.D.I. character sheets.

Simlas only accesses sheets that have been deliberately shared with the service account or otherwise made accessible through the configured Google integration.

C.O.D.I. remains the source of character-sheet values for features that depend on it. Simlas does not claim ownership of user-created character-sheet content.

## 3. How information is used

Information is processed only for purposes related to operating Simlas, including:

- linking Discord users to games and characters;
- executing commands;
- maintaining persistent game and encounter state;
- reading or updating authorized C.O.D.I. data;
- preventing duplicate or replayed game actions;
- diagnosing errors and maintaining application reliability;
- supporting development and testing.

## 4. Data sharing

Simlas does not sell personal information.

Information may be processed by services required for Simlas to operate, including:

- Discord;
- Google services used for C.O.D.I. access;
- infrastructure used to host Simlas and its persistent data.

Information may also be visible to other participants in the same game where that is necessary for normal gameplay, such as character names, combat results, conditions, and encounter state.

## 5. Message content

Simlas is primarily designed around Discord application commands and interactions.

If Discord Message Content access is enabled for compatibility with legacy features, Simlas may technically receive message content within the scope permitted by Discord. Simlas does not use ordinary conversation content for unrelated profiling, advertising, or sale.

The application aims to minimize privileged Discord data access as development progresses.

## 6. Data retention

Persistent data is retained for as long as it is needed to provide game continuity, maintain audit and transaction safety, or support active development and testing.

Historical game or encounter records may remain stored after an individual session ends unless they are removed through available administrative tools or a deletion request.

Backups may temporarily retain previously deleted information until normal backup rotation removes it.

## 7. Data deletion requests

A user may request deletion of information associated with their use of Simlas.

Because some records are part of shared game history, deletion may require distinguishing between:

- personal account associations that can be removed;
- shared historical game records that may need to be anonymized or retained for integrity.

Deletion requests should be sent to the Simlas administrator through the public project contact method listed in the Simlas documentation repository.

## 8. Security

Reasonable technical and organizational measures are used to protect Simlas data, including:

- keeping secrets and credentials outside the public source repository;
- restricting access to the runtime database and Google credentials;
- maintaining backups;
- limiting application permissions where practical.

No internet-connected service can guarantee absolute security.

## 9. Children and minimum age

Simlas is intended for users who are permitted to use Discord under Discord's applicable Terms of Service and minimum-age requirements.

## 10. Changes to this policy

This Privacy Policy may be updated as Simlas develops, particularly if its hosting model, public availability, integrations, or data practices change.

Material changes will be reflected in this document with an updated effective date.

## 11. Contact

Privacy or deletion requests may be submitted through the public Simlas documentation repository:

https://github.com/onibocho3281/simlas-docs
