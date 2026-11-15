# SpendWise — Security and data privacy

This repository contains the **static JavaScript edition** of SpendWise. It does not use a backend, server database, or user accounts.

## Storage and privacy

- Transactions are stored in browser **localStorage** under `spendwise_transactions_v1`.
- Records are accessible to anyone using the **same browser profile**, and potentially to extensions with appropriate permissions.
- Transactions do **not** automatically sync between computers, phones, or browser profiles.
- Browser storage can be deleted when site data is cleared, browser profiles are removed, or private/incognito sessions end.
- The website validates transaction amounts and creates text nodes rather than inserting user input as raw HTML.

## Backup safety

Use **Export Backup** regularly. Store the exported JSON file securely, preferably in a separate storage location. Importing JSON **replaces** all current transactions, so back up before importing.

## Not a production financial service

This is a learning/portfolio project. It has no authentication, encryption of locally stored transactions, account recovery, server backups, or professional financial controls. Avoid storing sensitive or business-critical data until appropriate security and persistence are implemented.

## Secrets

Never commit passwords, API tokens, `.env` files with secrets, service account credentials, or personal financial data to this repository.
