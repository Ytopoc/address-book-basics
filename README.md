# Address Book — OOP Basics

Foundation iteration of the address-book exercise: an OOP design with `Field`, `Name`, `Phone`, `Record`, and `AddressBook(UserDict)` classes. Contacts are kept in memory; later weeks add birthdays, persistence, and a Telegram bot on top.

## Stack

- Python 3.12 (standard library only)

## Classes

- **`Field`** — base class for any value stored on a record
- **`Name(Field)`** — required, non-empty string
- **`Phone(Field)`** — exactly 10 digits, validated on creation
- **`Record`** — owns one `Name` and a list of `Phone`s; supports `add_phone`, `remove_phone`, `edit_phone`, `find_phone`
- **`AddressBook(UserDict)`** — keyed by `Name.value`; supports `add_record`, `find`, `delete`

## Run

```bash
python hw6.py
```

The bottom of the file contains a small demo that creates a couple of records and exercises the API.
